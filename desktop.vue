<template>
    <div>
        
        <h1> select path</h1>
        <select>
            <option>Desktop</option>
            <option>Documents</option>
            <option>Downloads</option>
        </select>
        <input type="submit" value="Select">
        <button class="btn" @click="choose"> choose file</button>
        <ejs-uploader id='fileUpload' v-bind:multiple='true'></ejs-uploader>
    </div>
    <script>
    
        export default{

data()
{
    return {
        image:null
    }
}

            data()
            {
choose () {
  this.$refs.fileInput.click()
},
choose (event) {
  const files = event.target.files
  let filename = files[0].name  
  const fileReader = new FileReader()
  fileReader.addEventListener('load', () => {
    this.imageUrl = fileReader.result
  })
  fileReader.readAsDataURL(files[0])
  this.image = files[0]
}
            }
        }
        
        
        
           
               
               
               <script>       

    <style> 

    </style>
    