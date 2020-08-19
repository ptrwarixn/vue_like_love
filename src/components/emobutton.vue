<template>
<div>
    <div>
        <button v-on:click="$like" class="button-apple " id="blue"><i class="far fa-thumbs-up"></i></button>
        <button v-on:click="$love"  class="button-apple" id="pink"><i class="far fa-heart"></i></button>   
        <button v-on:click="$wow"  class="button-apple" id="yellow"><i class="far fa-surprise"></i></button>
        <button v-on:click="$haha" class="button-apple" id="orange"><i class="far fa-grin-squint"></i></button>
        <button v-on:click="$sad" class="button-apple" id="violet"><i class="far fa-sad-tear"></i></button>
        <button v-on:click="$angry"  class="button-apple" id="red"><i class="far fa-angry"></i></button>
        
        <h1>{{counter}}</h1>
       
    </div>
</div>
</template>

<script>
export default {
    name: 'emobutton',
    props: {
        label: String
    },
    data: function () {
        return {
            like: 0,
            love: 0,
            wow: 0, 
            sad:0,
            angry:0,
            counter:0
            
            
        };
    },
        methods:{
            $like:function(){
                this.counter +=1
                this.like +=1
                this.$emit('cc',this.counter)
            },
            $love:function(){
                this.counter +=10
                this.love +=1
                this.$emit('cc',this.counter)
            },
            $wow:function(){
                this.counter +=5
                this.wow += 1
                this.$emit('cc',this.counter)
            }, 
            $haha:function(){
                this.counter +=20
                this.haha += 1
                this.$emit('cc',this.counter)
            },
             $sad:function(){
                this.counter -=5
                this.sad += 1
                this.$emit('cc',this.counter)
            },
             $angry:function(){
                this.counter -=50
                this.angry += 1
                this.$emit('cc',this.counter)
            }
        }
        
    
}
</script>

<style>
    .button-apple{
    background-color: rgb(255, 252, 226);
    border: none;
    padding: 5px 5px 5px 5px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border-radius: 8px;
    border: 0.5px solid #ebebeb;
    width : 60px;
}
.button-apple-font-dd{
    background-color: white;
    border: none;
    color: #646363;
    padding: 5px 5px 5px 5px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border-radius: 8px;
    border: 0.5px solid #ebebeb;
    width : 60px;
}
button:hover#blue {
    color: blue;
}
button:hover#pink {
    color: rgb(255, 61, 174);
}
button:hover#yellow {
    color: yellow;
}
button:hover#orange {
    color: orange;
}
button:hover#violet {
    color: rgb(133, 0, 133);
}
button:hover#red {
    color:red;
}

</style>
