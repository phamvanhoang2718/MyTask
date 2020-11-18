

<template>
    <div id="app" class="container">
        <img src="https://scontent.fhan2-1.fna.fbcdn.net/v/t1.0-9/s960x960/104938038_2731154710449666_2018744051482241693_o.jpg?_nc_cat=102&ccb=2&_nc_sid=85a577&_nc_ohc=ydHqtAyaaSQAX_gOZhW&_nc_ht=scontent.fhan2-1.fna&tp=7&oh=4f8a6f2630a25b614bf2add4799f71ec&oe=5FD9774C" alt="" width="100"><span class="logo-title">Tết Tết Tết đến rồi!!!</span>
        <br>
        <div class="row">
            <div class="col-md-6"><ListTask></ListTask></div>
            <div class="col-md-6"><CompletedTask></CompletedTask></div>
        </div>
        <GetTask></GetTask>

    </div>
</template>

<script>
    import GetTask from './components/GetTask.vue'
    import ListTask from './components/ListTask.vue'
    import CompletedTask from './components/CompletedTask.vue'
    export default {
        components: {
            GetTask,
            ListTask,
            CompletedTask
        }
    
    }
</script>

<style>
  body {
    font-family: Helvetica, sans-serif;
  }
  ul li {
    list-style-type: none;
  }
  .logo-title {
    font-weight: bold;
  }
  .my-task {
    color: #f4f7f9!important;
    background-color: #656c7a!important;
  }
  
  .my-completed {
    color: #f4f7f9!important;
    background-color: #656c7a!important;
  }
  .task-length {
    float: right!important;
  }
  .completed-length {
    float: right!important;
  }
  .list-group-item {
    background-color: wheat;
  }
  .complete-list {
    background-color: #26bf0a!important;
  }
  .remove-completed {
    float: right!important;
  }
  .slide-fade-enter-active {
    transition: all .3s ease;
  }
  .slide-fade-leave-active {
    transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
  }
  
  .slide-fade-enter, .slide-fade-leave-to
  /* .slide-fade-leave-active below version 2.1.8 */ {
    transform: translateX(10px);
    opacity: 0;
  }
</style>