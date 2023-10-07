<template>
  <h2 class="basic">Hello from App</h2>
  <!-- <Reactivity />
  <hr>
  <Computed />
  <hr>
  <ClassAndStyleBinding />
  <hr>
  <ConditionalRendering/>
  <hr>
  <ListRendering/>
  <hr> -->
  <!-- <EventHandling/>
  <hr>
  <InputBindings/>
  <hr>
  <LifeCycle/>
  <hr/> -->
  <!-- <Watch/>
  <hr/>
  <TemplateRefs/>
  <hr/>
  <ComponentBasic/> -->
  <!-- <Props/> -->
  <!-- <EventParent/> -->
  <!-- <ComponentWithModel/> -->
  <!-- <FallthroughAttribute style="color:rgb(204, 11, 133)" class="parent-class" @click="console.log('from parent')"/> -->
  <!-- <Slots> New testdsf
    <span style="color:red">Click me!</span>
  </Slots>

<Slots>
  <template #header="headerSlots">
    {{ headerSlots }}
    <p>Header Content</p>
  </template>
  <template #default="defaultSlots">
    default Content {{ defaultSlots }}
  </template>
  <template #footer>
    <p>Footer Content</p>
  </template>
</Slots> -->
<!-- <ProvideInject/> -->
<button @click="showAsyncComponent = !showAsyncComponent"> Click to Show</button>

<div v-if="showAsyncComponent">
  <AsyncComponent />
</div>

</template>

<script setup>
import {provide, ref, defineAsyncComponent} from 'vue'
import Reactivity from './components/Reactivity.vue';
import Computed from './components/Computed.vue';
import ClassAndStyleBinding from './components/ClassAndStyleBinding.vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import ListRendering from './components/ListRendering.vue';
import EventHandling from './components/EventHandling.vue';
import InputBindings from './components/InputBindings.vue';
import LifeCycle from './components/LifeCycle.vue';
import Watch from './components/Watch.vue';
import TemplateRefs from './components/TemplateRefs.vue';
import ComponentBasic from './components/ComponentBasic.vue';
import Props from './components/Props.vue';
import Events from './components/Events.vue';
import EventParent from './components/EventParent.vue';
import ComponentWithModel from './components/ComponentVmodel.vue';
import FallthroughAttribute from './components/FallthroughAttribute.vue';
import Slots from './components/Slots.vue';
import ProvideInject from './components/ProvideInject.vue';


const msg = ref('Hello from provides');

const updateMessage = () => {
  msg.value = 'update message';
}

provide('message', {
  msg,
  updateMessage
})
provide('counter', ref(1))

const showAsyncComponent = ref(false);

const AsyncComponent = defineAsyncComponent(() => import('./components/AsyncComponent.vue'));

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
