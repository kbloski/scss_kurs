<template>
    <h1>Pętla while</h1>
    <div class="d1"></div>
    <div class="d2"></div>
    <div class="d3"></div>
    <div class="d4"></div>
    <div class="d5"></div>
    <div class="d6"></div>
</template>

<style lang="scss" scoped>
@use "sass:list";

$colors: gray, green, blue, yellow, #849920;


$n: 1; 

@while $n <= list.length($colors){
    .d#{$n}{
        background-color: list.nth($colors, $n );
    }

    $n: $n + 1;
}

div { 
    aspect-ratio: 1/1;
    border: 1px solid black;
    margin: 0 auto;
    width: 100px;
    margin-top: 1rem;
    background-color: list.nth($colors, 1);
}

</style>