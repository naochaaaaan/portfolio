<template>
    <div class="container">
        <div v-for="task in tasks" :key="task.id" class="accordion" id="accordionExample">
                <div class="card">
                    <div class="card-header" :id="'heading' + task.id">
                        <h5 class="mb-0">
                            <button v-if="task.id == 1" class="btn btn-link-dark" type="button" data-toggle="collapse" :data-target="'#collapse' + task.id" 
                            aria-expanded="true" :aria-controls="'collapse' + task.id">
                            {{ task.title }}
                            </button>
                            <button v-else class="btn btn-link-dark collapsed" type="button" data-toggle="collapse" :data-target="'#collapse' + task.id"
                            aria-expanded="false" :aria-controls="'collapse' + task.id">
                            {{ task.title }}
                            </button>
                        </h5>
                    </div>
                    <div v-if="task.id == 1" :id="'collapse' + task.id" class="collapse show" :aria-labelledby="'heading' + task.id" data-parent="#accordionExample">
                        <div class="card-body">
                        {{ task.content }}
                        </div>
                    </div>
                    <div v-else :id="'collapse' + task.id" class="collapse" :aria-labelledby="'heading' + task.id" data-parent="#accordionExample">
                        <div class="card-body">
                        {{ task.content }}
                        </div>
                    </div>
                </div>
            </div>
    </div>
</template>

<script>
    export default {
    data: function () {
        return {
            tasks: []
        }
    },
    methods: {
        getTasks() {
            axios.get('/api/tasks')
                .then((res) => {
                    this.tasks = res.data;
                });
        },
        deleteTask(id) {
            axios.delete('/api/tasks/' + id)
                .then((res) => {
                    this.getTasks();
                });
        }
    },
    mounted() {
        this.getTasks();
    }
}
</script>