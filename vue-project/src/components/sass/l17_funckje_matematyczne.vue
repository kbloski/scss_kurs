<template>
    <h1>Funkcje matematyczne scss</h1>
    <div class="random">random</div>
    <div class="percentage">percentage</div>
    <div class="round">round</div>
    <div class="cell">cell</div>
    <div class="floor">floor</div>
    <div class="abs">abs</div>
    <div class="min">min</div>
    <div class="max">max</div>
</template>

<style lang="scss" scoped>
@use 'sass:math';

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


$value: -1 * math.random();
.random::after {
    content: '#{$value}';
}

.percentage::after {
    content: '#{math.percentage($value)}';
}

.round::after {
    content: '#{math.round($value)}';
}

.cell::after {
    content: '#{math.ceil($value)}';
}

.abs::after {
    content: '#{math.abs($value)}';
}
.min::after {
    content: '#{math.min($value, -2, -3, -3.3)}';
}

.max::after {
    content: '#{math.max($value, 1, 2,3,4,5)}';
}


</style>