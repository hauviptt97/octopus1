<script setup>

</script>

<template>
    <div id="links"  v-bind:style="{ backgroundImage: 'url(' + $image('/src/assets/', 'octopusbg3.jpg') + ')' } " class="bg">
    <div class="homeContent">
        <a-row>
            <a-col :span="24">
                <span class="title">ABOUT ME</span>
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
}
</style>
