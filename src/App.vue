<template>
  <div class="container">
  <div class="row">
  <div class="col-md-6 col-md-offset-3">
  <br><br>
  <button class="btn-sm btn btn-primary" @click="selected = 'appMemory'">appMemory </button>
    <button class="btn-sm btn btn-primary" @click="selected = 'appNewMemory'">appNewMemory </button>
  <button class="btn-sm btn btn-primary" @click="selected = 'appAuthor'"> appAuthor </button>
  <br><br>
  <hr></hr>
<p> {{ selected }}</p>
<hr></hr>

<component :is="selected">
<h1 slot="heading">nice day</h1>
<p slot="content">It was a beautiful moment... </p>
</component>

    </div>
</div>
   </div>
</template>

<script>
import memory from './components/memory'
import NewMemory from './components/NewMemory'
import Author from './components/Author'

export default {
  data(){
    return{
      selected:"appMemory"
    }
  },
components: {
  appMemory:memory,
  appNewMemory:NewMemory,
  appAuthor:Author
} 
}
</script>

