<template>
    <h1>Pętla for</h1>
    <div class="d1"></div>
    <div class="d2"></div>
    <div class="d3"></div>
    <div class="d4"></div>
    <div class="d5"></div>
    <div class="d6"></div>
</template>

<style lang="scss" scoped>
$colors: red, green, blue, yellow, #849920;

// @for $i from 1 through 6{
//     .d#{$i} {
//         background-color: if( length($colors) >= $i, nth($colors, $i ), purple);
//     }
// }

@for $i from 1 through length($colors){
    .d#{$i} {
        content: '#{$i}';
        background-color: nth($colors, $i );
    }
}

div {
    aspect-ratio: 1/1;
    border: 1px solid black;
    margin: 0 auto;
    width: 100px;
    margin-top: 1rem;
    background-color: nth($colors, 1);
}

</style>