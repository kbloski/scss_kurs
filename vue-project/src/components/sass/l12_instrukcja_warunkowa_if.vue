<template>
    <h1>Instrukcja wartunkowa if</h1>
    <div></div>
    <div class="div1"></div>
</template>

<style lang="scss" scoped>
// $a: null;
// $b: true;
$a: 30;
$b: 310;

@function getColor($num1, $num2){
    // @if($a or $b){
    //     @return blue;
    // }

    @if($a > $b){
        @return red;
    }

    @else if($a < $b){
        @return green;
    }

    @return gray;
}

div {
    aspect-ratio: 1/1;
    width: 300px;
    background-color: getColor($a, $b );
    margin: 0 auto;
}

.div1 {
    margin-top: 1rem;
    // background-color: if(warunek, wartość jeśli prawda, wartość jeśli fałsz);
    background-color: if($a > $b, green, red);
}

</style>