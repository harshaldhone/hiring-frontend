<template>
    <div v-if="type==='text'">

        <div class="grid-item">
            <div>
                <label for="fname">{{Label}}<span class="Optional"> {{SubLabel}}</span></label>
            </div>
            <div>
                <input :type=type :id=inputId name="fname"> 
            </div>   
        </div>
    </div>
    <div v-else-if="type==='file'">
        <div class="grid-item">
            <div>
                <label for="fname">{{Label}}<span class="Optional"> {{SubLabel}}</span></label>
            </div>
            <div>
                <input :type=type :id=inputId name="fname"> 
            </div>   
        </div>
    </div>
    <div v-else-if="type==='textarea'">
        <div class="grid-item">
            <div>
                <label for="fname">{{Label}}<span class="Optional"> {{SubLabel}}</span></label>
            </div>
            <div>
                <textarea :id=inputId name="fname"> </textarea>
            </div>   
        </div>
    </div>
</template>
<script>

export default {
    name:'Input',
    props:{
        Label:String,
        SubLabel:String,
        type:String,
        inputId:String
    },
    
    
}
</script>

<style>

.grid-item {
  padding: 20px;
  font-size: 20px;
  text-align: left;
}
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=file] {
  width: auto;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  display: flex;
}
::-webkit-file-upload-button{
    padding: 13px 20px;
    
}

textarea{
    width: 100%;
    padding: 13px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    height: 100px;
    
}
.Optional{
  font: 0.8rem/1.0 "PT Sans", Arial, sans-serif;
  color: #5a5a5a;
}
</style>