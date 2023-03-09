<template>
    <div class="oran active"></div>
</template>

<script>
export default{
    name:'OrangeInput',
    components:{

    }
}
</script>

<style scoped lang="scss">
.oran {
    height: 16px;
    width: 16px;
    border-radius: 10px;
    border: 1px solid black;
    background-color: white;
    margin-right: 1rem;
}

.oran.active {
    border: 3px solid #FFA200;
}
</style>