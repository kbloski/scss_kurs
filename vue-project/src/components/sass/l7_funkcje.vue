<template>
    <!-- <div>Funkcje</div> -->
    <div id="p1"></div>
    <div id="p2"></div>
    <div id="p3"></div>
    <div id="p4"></div>
</template>

<style lang="scss" scoped>
$height-start: 400px;

@function divisiton($a, $b){
    @return $a / $b;
}

div {
    height: $height-start;
    width: 50px;
    display: inline-block;
    background: green;
    margin-left: 1rem;
}

#p1 {
    // przy wywołaniu nawiasy muszą być sklejone z funkcją
    
    height: divisiton($height-start, 1);
}
#p2 {
    height: divisiton($height-start, 2);
}
#p3 {
    height: divisiton($height-start, 3);
}
#p4 {
    height: divisiton($height-start, 4);
}

</style>