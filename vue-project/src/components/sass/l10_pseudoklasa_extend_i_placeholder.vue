<template>
    <div>Domieszki</div>
    <h1>Nagłówek1</h1>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit enim nostrum
        soluta eveniet molestias perferendis sapiente quos voluptates! Explicabo soluta ea
        pariatur doloremque laboriosam optio vitae, quas necessitatibus unde autem!
    </p>
    <h2>Nagłówek2</h2>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit enim nostrum
        soluta eveniet molestias perferendis sapiente quos voluptates! Explicabo soluta ea
        pariatur doloremque laboriosam optio vitae, quas necessitatibus unde autem!
    </p>
    <h3>Nagłówek3</h3>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit enim nostrum
        soluta eveniet molestias perferendis sapiente quos voluptates! Explicabo soluta ea
        pariatur doloremque laboriosam optio vitae, quas necessitatibus unde autem!
    </p>
    <h4>Nagłówek4</h4>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit enim nostrum
        soluta eveniet molestias perferendis sapiente quos voluptates! Explicabo soluta ea
        pariatur doloremque laboriosam optio vitae, quas necessitatibus unde autem!
    </p>
</template>

<style lang="scss" scoped>
// STRUKTURA DOMIESZKI 
// @mixin nazwa {
//     ...
// }
// 
// Zagnieżdzanie domieszki
// @mixin nazwa2{ 
//  @include nazwa;
// }
// 
// Domieszki nie można umieszczać w ciele innej domieszki

$margin-1: 30px;
$margin-2: 25px;

@mixin text-align {
    text-align: justify;
}

// extend tworzy odatkowe klasy które rozszerzają inne klasy co w kompilacji może zaśmiecać kod
.padding-and-align
{
    padding: 0px 20px 0px 20px;
    @include text-align
}

// placeholder (nie tworzy zbędnych nazw klas)
%h1-h2
{
    font-family: "Arial";
    margin-top: $margin-1;
    margin-bottom: $margin-1;
    color: #333;
}

%h3-h4
{
    font-family: "Verdana";
    margin-top: $margin-2;
    margin-bottom: $margin-2;
    color: #555;
}

h1, h2 {
    @extend .padding-and-align;
    @extend %h1-h2;
}
h1 {
    font-size: 40px;
}

h2 {
    font-size: 35px;
}

h3, h4 {
    @extend .padding-and-align;
    @extend %h3-h4;
}

h3 {
    font-size: 27px;
}

h4 {
    font-size: 20px;
}

p {
    color: #555;
    @extend .padding-and-align;
}

</style>