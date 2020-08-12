<template>
    <div class="container mb-4">
        <div class="row">
            <div class="col-4">
                <!-- list -->
                <div class="list-group" id="myList" role="tablist">
                    <a class="list-group-item list-group-item-action list-group-item-secondary active" data-toggle="list" href="#profile" role="tab">プロフィール</a>
                    <a class="list-group-item list-group-item-action list-group-item-secondary" data-toggle="list" href="#license" role="tab">資格</a>
                    <a class="list-group-item list-group-item-action list-group-item-secondary" data-toggle="list" href="#hobby" role="tab">趣味・特技</a>
                    <a class="list-group-item list-group-item-action list-group-item-secondary" data-toggle="list" href="#computer" role="tab">愛用PC</a>
                </div>
            </div>
            <div class="col-8">
                <!-- contents -->
                <div class="tab-content">
                    <!-- profile -->
                    <div class="tab-pane active" id="profile" role="tabpanel">
                        <p>氏名     :   松木 直也</p>
                        <p>出身     :   北海道函館市</p>
                        <p>現住所   :   北海道札幌市</p>
                        <p>生年月日 :   1984年5月1日</p>
                        <p>年齢     :   36歳</p>
                        <p>血液型   :   A型</p>
                    </div>
                    <!-- license -->
                    <div class="tab-pane" id="license" role="tabpanel">
                        <p>実用英語検定2級</p>
                        <p>第1種普通自動車免許</p>
                        <p>福祉有償運送乗務員講習 修了</p>
                        <p>普通救命講習 修了</p>
                        <p>患者等搬送乗務員講習 修了</p>
                    </div>
                    <!-- hobby -->
                    <div class="tab-pane" id="hobby" role="tabpanel">
                        <p>PC自作</p>
                        <p>料理</p>
                        <p>美味しいもの食べ歩き</p>
                        <p>音楽鑑賞</p>
                        <p>楽器を弾くこと</p>
                        <p>あてのないドライブ</p>
                        <p>古着屋巡り</p>
                        <p>ゲーム</p>
                    </div>
                    <!-- computer -->
                    <div class="tab-pane" id="computer" role="tabpanel">
                        <p>CPU:AMD Ryzen 7 2700X</p>
                        <p>CPUクーラー:COOLER MASTER MASTERAIR MA410P</p>
                        <p>メモリ:メーカー不明 DDR4 16GB</p>
                        <p>M/B:msi B450 GAMING PLUS MAX</p>
                        <p>G/B:MSI GeForce GTX 1070</p>
                        <p>サウンドカード:CREATIVE Sound Blaster ZxR SB-ZXR-R2</p>
                        <p>SSD:メーカー不明 128GB×1 256GB×1</p>
                        <p>HDD:Western Digital 1TB×1 2TB×2</p>
                        <p>ドライブ:pioneer BD-206</p>
                        <p>ケース:InWin INW-509-BXR148</p>
                        <p>電源:COOLER MASTER V750 platina</p>
                        <p>OS:microsoft windows10 home edition</p>
                        <p>モニター:MITSUBISHI diamondcrysta 24インチ<br>
                                            LG ウルトラワイド 24インチ</p>
                        <p>アンプ:自作真空管アンプ</p>
                        <p>スピーカー:ONKYO PS-33X</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>