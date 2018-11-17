<template>
    <div>
        <p>Masiv: {{ array }} </p>
        <p>Summa: {{ getSum() }} </p>
    </div>
</template>

<script>
export default {
    data (){
        return{
            result: 0,
            array: [10, 7, 9, 4, 10, 7, 2]
        }
    },
 methods: {
        getSum () {
            var _result = 0;
            for (var i = 0; i < this.array.length; i++) {
                _result += this.array[i]
         }
           return _result;
        }
    } 
}
</script>



