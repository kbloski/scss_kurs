<template>
    <h1>Pętla Each</h1>
    <div class="d1"></div>
    <div class="d2"></div>
    <div class="d3"></div>
    <div class="d4"></div>
    <div class="d5"></div>
    <div class="d6"></div>
</template>

<style lang="scss" scoped>
$colors: gray, green, blue, yellow, #849920;

// ########## Petla 1
$item: 1;
@each $color  in $colors {
    .d#{$item}{
        background-color: $color;
    }
    $item: $item+1;
}

// ########## Petla 2
$item: 1;
@each $color in (gray, green, blue, yellow, #849920, orange) {
    .d#{$item}{
        background-color: $color;
    }
    $item: $item+1;
}


// ########## Petla 3
$i: 1;
@each $color, $boder, $width, $height in 
                                        ( red, 1px, 30px, 20px ),
                                        ( white, 2px, 10px, 20px ),
                                        ( aqua, 3px, 20px, 20px ),
                                        ( blue, 4px, 40px, 20px ),
                                        ( purple, 5px, 50px, 20px ),
                                        ( yellow, 6px, 60px, 20px )
{
    
    .d#{$i}{
        width: $width;
        height: $height;
        border: $boder solid $color;
    }

    $i: $i + 1;
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