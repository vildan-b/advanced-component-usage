<template>
  <div class="container">
  <div class="row">
  <div class="col-md-6 col-md-offset-3">
    <app-memory>
    <h1 slot="heading">nice day</h1>
    <p slot="content">It was a beautiful moment... </p>
    </app-memory>
    
    </div>
</div>
   </div>
</template>

<script>
import memory from './memory'
export default {
components: {
  appMemory:memory
} 
}
</script>

