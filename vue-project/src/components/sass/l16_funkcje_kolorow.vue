<template>
    <h1>Funkcje wbudowane</h1>
    <div class="d1 rgb">1</div>
    <div class="d2 rgba">2</div>
    <div class="d3 red_green_blue">3</div>
    <div class="d4 mix">4</div>
    <div class="d5">5</div>
    <div class="d6">6</div>
</template>

<style lang="scss" scoped>
div {
    aspect-ratio: 1/1;
    border: 1px solid black;
    margin: 0 auto;
    width: 100px;
    margin-top: 1rem;
    background-color: rgb(194, 194, 194);
    text-align: center;
    font-size: 20px;
}

@function rgbFunction(){
    @return rgb(255,11,25)
};

@function colorRgb(){
    @return rgb(red(#ca3827), green(#00ca33), blue(#ca38aa));
};

.rgb {
    background-color: rgbFunction();
}

.rgba {
    background-color: rgb(255,11,25, .2);
}

.red_green_blue {
    // funkcje red() green() blue() pobierają zmienne z kolorów odpowiadające
    background-color: colorRgb()
}

.mix {
    // mieszanie kolorów
    background-color: mix(red, blue);
}


</style>