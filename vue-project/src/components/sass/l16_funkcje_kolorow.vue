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
@use 'sass:color';

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

// Funkcja rgbFunction poprawiona
@function rgbFunction() {
    @return rgb(255, 11, 25);
}

@function colorRgb() {
    @return rgb(
        color.channel(#ca3827, 'red'),
        color.channel(#00ca33, 'green'),
        color.channel(#ca38aa, 'blue')
    );
}

// Klasy z poprawionymi wartościami kolorów
.rgb {
    background-color: rgbFunction();
}

.rgba {
    background-color: rgba(255, 11, 25, 0.2); // Użycie rgba zamiast rgb dla przezroczystości
}

.red_green_blue {
    background-color: colorRgb();
}

.mix {
    background-color: color.mix(red, blue); // Użycie funkcji z modułu 'color'
}



</style>