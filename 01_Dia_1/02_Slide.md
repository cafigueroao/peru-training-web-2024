---
layout: page
title: Día 2
parent: Martes 2 de julio
nav_order: 2
---
<style>
  html {
    box-sizing: border-box;
  }
  *, *:before, *:after {
    box-sizing: inherit;
  }
  
  @mixin center() {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  body {
    margin: 0;
    height: 100vh;
    @include center;
  }
  
  .container {
    position: relative;
    width: 900px;
    height: 600px;
    border: 2px solid white;
    .img {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-size: 900px 100%;
    }
    .background-img {
      background-image: url('https://i.imgur.com/s08MkXC.jpg');
    }
    .foreground-img {
      background-image: url('https://i.imgur.com/PfIWek4.jpg');
      width: 50%;
    }
    
    .slider {
      position: absolute;
      -webkit-appearance: none;
      appearance: none;
      width: 100%;
      height: 100%;
      background: rgba(#f2f2f2, .3);
      outline: none;
      margin: 0;
      transition: all .2s;
      @include center;
      &:hover {
        background: rgba(#f2f2f2, .1);
      }
      &::-webkit-slider-thumb {
        -webkit-appearance: none;
        appearance: none;
        width: 6px;
        height: 600px;
        background: white;
        cursor: pointer;
      }
      &::-moz-range-thumb {
        width: 6px;
        height: 600px;
        background: white;
        cursor: pointer;
      }
    }
    
    .slider-button {
      $size: 30px;
      pointer-events: none;
      position: absolute;
      width: $size;
      height: $size;
      border-radius: 50%;
      background-color: white;
      left: calc(50% - 18px);
      top: calc(50% - 18px);
      @include center;
      
      @mixin arrow-helper() {
        content: '';
        padding: 3px;
        display: inline-block;
        border: solid #5D5D5D;
        border-width: 0 2px 2px 0;
      }
      &:after {
        @include arrow-helper();
        transform: rotate(-45deg);
      }
      &:before {
        @include arrow-helper();
        transform: rotate(135deg);
      }
    }
  }
</style>
<script>
  $("#slider").on("input change", (e)=>{
    const sliderPos = e.target.value;
    // Update the width of the foreground image
    $('.foreground-img').css('width', `${sliderPos}%`)
    // Update the position of the slider button
    $('.slider-button').css('left', `calc(${sliderPos}% - 18px)`)
  });
</script>
# Prueba de control deslizante de imagen de antes/después
<div class='container'>
  <div class='img background-img'></div>
  <div class='img foreground-img'></div>
  <input type="range" min="1" max="100" value="50" class="slider" name='slider' id="slider">
  <div class='slider-button'></div>
</div>