<script setup>
</script>

<template>
    <div  id="home" v-bind:style="{ backgroundImage: 'url(' + $image('/public/', 'octopusbg.jpg') + ')' } " class="bg">
        <div class="homeContent">
<a-row>
    <a-col :span="24">
        <span class="title">Octopus</span>
    </a-col>
</a-row>
<a-row>
    <a-col :span="24">
        The return of Ocean ruler
    </a-col>
</a-row>
<a-row>
    <a-col :span="24">
        Contract: <span style="font-weight: 500; font-style: italic; font-size: 1vw; ">0x69Ed89ecd35082E031fE52b75123F801DB083306</span>
    </a-col>
</a-row>
<a-row justify="center">
    <a-col :span="4">
        <a href="https://app.uniswap.org/" target="_blank"><button>
            BUY $OCTOPUS
        </button>
        </a>
    </a-col>
    <a-col :span="1">
    </a-col>
    <a-col :span="4">
        <a href="https://www.dextools.io/app/en/ether/pair-explorer/0x843f86e8a97f11ad4560444071ca35a9783bd8a9" target="_blank">
        <button>
            VIEW CHART
        </button>
        </a>
    </a-col>
</a-row>
<a-row  justify="center">
    <a-col :span="2">
        <a href="https://web.telegram.org/" target="_blank"><i class="fa-brands fa-telegram"></i></a>
    </a-col>
    <a-col :span="2">
        <a href="https://twitter.com/" target="_blank"><i class="fa-brands fa-twitter"></i></a>
    </a-col>
    <a-col :span="2">
        <a href="https://www.linkedin.com/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
    </a-col>
    <a-col :span="2">
        <a href="https://discord.com/" target="_blank"><i class="fa-brands fa-discord"></i></a>
    </a-col>
</a-row>
</div>
    </div>
    

</template>

<style>
.bg {
    width: 100%;
    height: 105vh;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
}

.homeContent{
    margin-top: 30vh;
}

#home .ant-row {
    margin-bottom: 3vh;
}

.ant-row .ant-col {
    text-align: center;
    color: #fff;
}

#home .ant-row i {
    font-size: 2vw;
    color: #fff;
}

.title {
    font-size: 6vw;
    font-weight: 800;
    font-family: 'Courier New', Courier, monospace;
    color: aliceblue;
}
</style>
