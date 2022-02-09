<template>
  <ul>
    <li
      v-for="(el, index) in elements"
      class="dot"
      :key="index"
      :class="{'dot-selected': currentElement === index}"
    >
      <button
        class="indicator-btn"
        @click="$emit('mostra',index)"
        :disabled=" currentElement === index"
      />
    </li>
  </ul>
</template>

<script>
export default {
    props: { 
        elements: Array, 
        currentElement: Number, 
        
    }
}
</script>

<style lang="scss" scoped>
ul{
    display: inline-block;
    .dot {
        height: 20px;
        width: 20px;
        border-radius: 50%;
        background: black;
        opacity: 0.2;
        cursor: pointer;
        position: relative;
    }
    
    .dot-selected {
        opacity: 0.7;
        cursor: default;
    }
    
    .indicator-btn {
        position: absolute;
        left: 0px;
        padding: 0px;
        height: 100%;
        width: 100%;
        border-radius: 50%;
        background: transparent;
        border: none;
        cursor: pointer;

    }
}
</style>