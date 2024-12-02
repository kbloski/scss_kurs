<template>
    <div>Elementy listy:</div>
    <div>Długość listy:</div>
    <div>Pierwszy el listy:</div>
    <div>Drugi el listy:</div>
    <div>Ostatni el listy:</div>
    <div>Drugi el zagnieżdzonej listy pod indexem 2:</div>
</template>

<style lang="scss" scoped>
@use 'sass:list';
// indexy listy zaczynają się od 1 nie, jak w innych językach od 0


$list: 14, 21 3 4 5, 10, (222, 22, 2221, 22222); // lista wartości
$length: list.length($list); // długość listy
$first: list.nth($list, 1); // wybór elementu listy
$second: list.nth($list, 2);
$last: list.nth($list, 3);
$list2-second-el: list.nth(list.nth($list, 2), 2); // drugi el zagnieżdzonej listy

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