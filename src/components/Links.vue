<script setup>

</script>

<template>
    <div id="links"  v-bind:style="{ backgroundImage: 'url(' + $image('/public/', 'octopusbg2.jpg') + ')' } " class="bg">
    <div class="homeContent">
        <a-row>
            <a-col :span="24">
                <span class="title">SOCIAL LINKS</span>
            </a-col>
        </a-row>
        <a-row justify="center">
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
#links .ant-row .ant-col {
    text-align: center;
}

#links .ant-row i {
    font-size: 4vw;
    color: #fff;
}
</style>
