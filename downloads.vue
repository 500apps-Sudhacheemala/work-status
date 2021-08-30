<template>
    
</template>
<script>

export default{

data()
{
    return {

                   
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
}
            
        
        
        
        
           

               
               </script>       

    <style> 

    </style>
    