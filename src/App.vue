<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button v-on:click="currentTemplate = 'appBlue'" class="btn btn-primary">Load Blue Template</button>
                <button v-on:click="currentTemplate = 'appGreen'" class="btn btn-success">Load Green Template</button>
                <button v-on:click="currentTemplate = 'appRed'" class="btn btn-danger">Load Red Template</button>
                <hr>
                <component v-bind:is="currentTemplate">
                  <h1>Fallback content</h1>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nostrum, officia.</p>
                </component>
            </div>
        </div>
    </div>
</template>

<script>
    import Blue from './components/Blue.vue';
    import Green from './components/Green.vue';
    import Red from './components/Red.vue';

    export default {
      data(){
        return {
          currentTemplate: ''
        }
      },
        components: {
            appBlue: Blue,
            appGreen: Green,
            appRed: Red
        }
    }
</script>

<style>
</style>
