<template>
    <div>Elementy listy:</div>
    <div>Długość listy:</div>
    <div>Pierwszy el listy:</div>
    <div>Drugi el listy:</div>
    <div>Ostatni el listy:</div>
    <div>Drugi el zagnieżdzonej listy pod indexem 2:</div>
</template>

<style lang="scss" scoped>
$list: 14, 21 3 4 5, 10, (222, 22, 2221, 22222); // lista wartości
$length: length($list); // długość listy
$first: nth($list, 1); // wybór elementu listy
$second: nth($list, 2);
$last: nth($list, 3);
$list2-second-el: nth(nth($list, 2), 2); // drugi el zagnieżdzonej listy

$elementTag: div;

#{$elementTag}:nth-child(1)::after {
    content: '#{$list}';
}
#{$elementTag}:nth-child(2)::after {
    content: '#{$length}';
}
#{$elementTag}:nth-child(3)::after {
    content: '#{$first}';
}
#{$elementTag}:nth-child(4)::after {
    content: '#{$second}';
}
#{$elementTag}:nth-child(5)::after {
    content: '#{$last}';
}
#{$elementTag}:nth-child(#{5+1})::after {
    content: '#{$list2-second-el}';
}

</style>