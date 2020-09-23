<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button class="btn btn-primary" @click="selectedComponent='appBlue'">Load Blue Template</button>
                <button class="btn btn-success" @click="selectedComponent='appGreen'">Load Green Template</button>
                <button class="btn btn-danger" @click="selectedComponent='appRed'">Load Red Template</button>

                <component  :is="selectedComponent">
                  <h1 slot="title">what a day</h1>
                  <p slot="content">Sometyimes does make sense to keep a job that does not make sense in you ?</p>
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
        return{
          selectedComponent:'appBlue'
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
button{
  margin-right: 5px;
}
</style>
