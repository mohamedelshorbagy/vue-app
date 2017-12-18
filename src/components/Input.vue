<template>
    <div class="root">
            <hr>
            <input class="form-control" v-if="type === 'input'" :type="elementType" :placeholder="pc" />
            <div v-if="type === 'textarea'">
                <textarea class="form-control"  :rows="rows" cols="30" :placeholder="pc"></textarea>
            </div>
            <select class="form-control" v-if="type === 'select'">
                <option v-for="opt in elOpts" :value="opt">{{ opt }}</option>
            </select>


    </div>




</template>



<script>

export default {
    props:['type','elementType','rows','pc','elOpts'],
    data() {
        return {
            message:'',
            show:false
        }
    },
    methods: {
    }
}

</script>


<style scoped>

textarea {
    margin-bottom: 15px;
    margin-top: 15px;
    resize:none;
}

.btn {
    margin-bottom:15px;
}


</style>