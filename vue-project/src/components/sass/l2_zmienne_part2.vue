<template>
    <div class="image-1"></div>
    <div class="image-2"></div>
    <div class="image-3"></div>
    <div class="image-4"></div>
</template>

<style lang="scss" scoped>

$div-width: 400px;
$div-height: 267px;
$div-border: 2px solid #555;

$images-main-folder: '/public/images';
$color-or-greyscale: 'color';
$color-or-greyscale: 'greyscale';
$ext: 'jpg';

$image-1-name: '01';
$image-2-name: '02';
$image-3-name: '03';
$image-4-name: '04';

// dynamic path 
$image-1: url('#{$images-main-folder}/#{$color-or-greyscale}/#{$image-1-name}.#{$ext}');
$image-2: url('#{$images-main-folder}/#{$color-or-greyscale}/#{$image-2-name}.#{$ext}');
$image-3: url('#{$images-main-folder}/#{$color-or-greyscale}/#{$image-3-name}.#{$ext}');
$image-4: url('#{$images-main-folder}/#{$color-or-greyscale}/#{$image-4-name}.#{$ext}');

$b-img: background-image;
$div-element: div;

$class-1: 'image-1';
$class-2: 'image-2';
$class-3: 'image-3';
$class-4: 'image-4';

// dynamic name class
#{$div-element} {
    width: $div-width;
    height: $div-height;
    display: inline-block;
    border: $div-border;
    margin: 4px*2;

    background-repeat: no-repeat;
    background-size: cover;
}

.#{$class-1}{

    // dynamic name properties
    #{$b-img}: $image-1;
}
.#{$class-2}{
    #{$b-img}: $image-2;
}
.#{$class-3}{
    #{$b-img}: $image-3;
}
.#{$class-4}{
    #{$b-img}: $image-4;
}



</style>