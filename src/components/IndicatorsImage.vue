<template>
  <ul class="indicators">
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
.indicators{
    display: inline-block;
    border-bottom: 1px solid black;
    padding-bottom:15px ;
    margin: 15px 0;
    .dot {
        height: 20px;
        width: 20px;
        border-radius: 50%;
        background: black;
        opacity: 0.3;
        position: relative;
        display: inline-block;
        margin: 0 30px;
    }
    
    .dot-selected {
        opacity: 1;
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