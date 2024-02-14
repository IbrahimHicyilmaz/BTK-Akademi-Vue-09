<template>
    <div>
        <h1>Öğrenciler</h1>
        <div v-for="student in students" :key="student.id">
            <router-link :to="{name:'studentInfo',params:{id:student.id}}">{{ student.name }}</router-link>
        </div>
        <div>
    
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            students: [
                { id: 1, name: 'ibrahim', not: '95' },
                { id: 2, name: 'Varol', not: '85' },
                { id: 3, name: 'Ali', not: '75' },
            ]
        }
    },
}
</script>

<style>

</style>