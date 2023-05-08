<template>
     <div>
          <h2>About</h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sapiente quidem magni debitis illum totam molestiae, animi voluptas sed fugit exercitationem? Expedita dolor modi iure aperiam tenetur optio aliquam distinctio animi.</p>
          <div>
            {{ data }}
          </div>
     </div>
</template>

<script setup lang="ts">

const { data } = await useFetch('/api/ninja?name=mario', {
    method: 'post',
    body: {
        age: 30
    }
})

</script>

<style scoped></style>
