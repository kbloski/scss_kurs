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
    margin: $spacing/2;

    // zmiany nazw selektorów z &-dalsza-czesc-nazwy-klasy
    &-1 {
        &-1 {
            background: darken( $first-color, 10 * $n);
        };
        &-2 {
            background: darken( $first-color, 20 * $n);
        };
        &-3 {
            background: darken( $first-color, 30 * $n);
        }
    }

    &-2 {
        &-1 {
            background: darken($second-color, 10 *$n )
        };
        &-2 {
            background: darken($second-color, 20 *$n )
        };
        &-3 {
            background: darken($second-color, 30 *$n )
        }
    }

    &-3 {
        &-1 {
            background: darken($third-color, 10 *$n )
        };
        &-2 {
            background: darken($third-color, 20 *$n )
        };
        &-3 {
            background: darken($third-color, 30 *$n )
        }
    }

}


</style>