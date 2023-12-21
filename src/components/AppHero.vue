<script>
export default {
    data() {
        return {
            file_name: "obama.jpg"
        }
    },
    methods: {
        getImagePath(path) {
            return new URL(path, import.meta.url).href
        }
    },
}
</script>
<template lang="">
    <div>
        <img :src="getImagePath(`../assets/${file_name}`)" alt="obaaama" width="1000px">
    </div>
</template>
<style lang="">
    
</style>