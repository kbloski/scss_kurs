<template>
    <div>Tworzenie nazw selektórów za pomocą znaku @ jak w less</div>
    <div class="table">
        <div class="row">
            <div class="cell cell-1-1"></div>
            <div class="cell cell-2-1"></div>
            <div class="cell cell-3-1"></div>
        </div>
        <div class="row">
            <div class="cell cell-1-2"></div>
            <div class="cell cell-2-2"></div>
            <div class="cell cell-3-2"></div>
        </div>
        <div class="row">
            <div class="cell cell-1-3"></div>
            <div class="cell cell-2-3"></div>
            <div class="cell cell-3-3"></div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use 'sass:color';
@use 'sass:math';

$size: 100px;
$spacing: 2px;

$first-color: red;
$second-color: green;
$third-color: blue;

$n: 0.9;

.row {
    display: block;
}

.cell {
    width: $size;
    height: $size;
    display: inline-block;
    border: 1px solid #888;
    margin: math.div($spacing, 2); // Poprawa wyrażenia dzielenia

    // Zmiany nazw selektorów z &-dalsza-czesc-nazwy-klasy
    &-1 {
        &-1 {
            background: color.adjust($first-color, $lightness: 10 * $n * 1%);
        }
        &-2 {
            background: color.adjust($first-color, $lightness: 20 * $n * 1%);
        }
        &-3 {
            background: color.adjust($first-color, $lightness: 30 * $n * 1%);
        }
    }

    &-2 {
        &-1 {
            background: color.adjust($second-color, $lightness: 10 * $n * 1%);
        }
        &-2 {
            background: color.adjust($second-color, $lightness: 20 * $n * 1%);
        }
        &-3 {
            background: color.adjust($second-color, $lightness: 30 * $n * 1%);
        }
    }

    &-3 {
        &-1 {
            background: color.adjust($third-color, $lightness: 10 * $n * 1%);
        }
        &-2 {
            background: color.adjust($third-color, $lightness: 20 * $n * 1%);
        }
        &-3 {
            background: color.adjust($third-color, $lightness: 30 * $n * 1%);
        }
    }
}
</style>
