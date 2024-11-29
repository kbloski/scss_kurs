<template>
    <div>Domieszki z parametrami</div>

    <div class="level-1">
        <div class="level-2">
            <div class="level-3">
                <p><span>akapit</span></p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

@mixin b-line {
    border-width: 5px;
    border-style: solid;
}

@mixin b-color ($color, $bg-color) {
    border-color: $color;
    background: $bg-color;
}

@mixin margins ($par1: 1px 2px 3px 4px, $par2: 5px 6px 7px 8px){
    margin: $par1;
    padding: $par2;
}

.level-1,
.level-2,
.level-3 {
    @include b-line();
    @include margins();
}

.level-1 {
    @include b-color(yellow, grey);
}
.level-2 {
    @include b-color(red, blue);
    @include margins(1px);
}
.level-3 {
    @include b-color(blue, aqua);

    p {
        @include margins(2rem, 2rem);

        span {
            padding: 5px;
            box-shadow: 4px 4px 4px black;
            @include b-color(black, yellow)
        }
    }
}
</style>