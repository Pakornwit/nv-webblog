<template>
    <h1>Get All Users</h1>
</template>
<script>
import UserService from '@/services/UsersSercice'

export default {
    async created () {
        let results = (await UserService.index()).data
        console.log(results)
    } 
    
}
</script>
<style scoped>


</style>