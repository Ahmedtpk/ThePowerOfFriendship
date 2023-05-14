<template>
     <div class="outerdiv">
         <div class="dark fire">
            <h1 class="Blazing" contenteditable="true">THE POWER OF FRIENDSHIP</h1> 
        </div>
      <img class="goku" src="~/assets/Goku.png" />

     </div>
</template>

<script setup lang="ts">


</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Akronim);

.goku{
    width: 400px;
}
.outerdiv {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

body {
    background: black;
}

.fire {
  margin: 20px auto;
  width: 80%;
  max-width: 1000px;
  height: 200px;

  background-position: center center;
  background-size: 1000px 200px;
  border-radius: 10px;
  font-family: 'Akronim';
  overflow: hidden;
    text-align: center;
  vertical-align: middle;

}
.fire:before {
  content: '';
  display: inline-block;
  height: 100%;
  vertical-align: middle;
}

.Blazing {
  display: inline-block;
  margin: 0;
  color: rgb(255, 115, 0);
  font-size: 70px;
  line-height: 50px;
  min-width: 50px;
  outline: none;
  vertical-align: middle;
    
  text-shadow:
        0 3px 20px blue,
        0 0 20px blue,
    0 0 10px orange,
    4px -5px 6px yellow,
    -4px -10px 10px yellow,
    0 -10px 30px yellow;
  animation: 2s Blazing infinite alternate linear;
}

@media only screen and (max-width: 600px) {
    .Blazing {
      background-color: aqua;
      width: 5px;
  }
}

@keyframes Blazing {
  0%   { text-shadow: 0 3px 20px blue, 0 0 20px blue,
    0 0 10px orange,
    0 0 0 yellow,
    0 0 5px yellow,
    -2px -5px 5px yellow,
    4px -10px 10px yellow; }
  25%   { text-shadow: 0 3px 20px blue, 0 0 30px blue,
    0 0 20px orange,
    0 0 5px yellow,
    -2px -5px 5px yellow,
    3px -10px 10px yellow,
    -4px -15px 20px yellow; }
  50%   { text-shadow: 0 3px 20px blue, 0 0 20px blue,
    0 -5px 10px orange,
    -2px -5px 5px yellow,
    3px -10px 10px yellow,
    -4px -15px 20px yellow,
    2px -20px 30px rgba(255,255,0,0.5); }
  75%   { text-shadow: 0 3px 20px blue, 0 0 20px blue,
    0 -5px 10px orange,
    3px -5px 5px yellow,
    -4px -10px 10px yellow,
    2px -20px 30px rgba(255,255,0,0.5),
    0px -25px 40px rgba(255,255,0,0)}
  100%   { text-shadow: 0 3px 20px blue, 0 0 20px blue,
    0 0 10px orange,
    0 0 0 yellow,
    0 0 5px yellow,
    -2px -5px 5px yellow,
    4px -10px 10px yellow; }
}
</style>