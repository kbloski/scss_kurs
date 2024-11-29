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

$margin-1: 30px;
$margin-2: 25px;

@mixin pading-adnd-aglin
{
    padding: 0px 20px 0px20px;
    text-align: justify;
}

@mixin h1-h2
{
    font-family: "Arial";
    margin-top: $margin-1;
    margin-bottom: $margin-1;
    color: #333;
}

@mixin h3-h4
{
    font-family: "Verdana";
    margin-top: $margin-2;
    margin-bottom: $margin-2;
    color: #555;
}

h1, h2 {
    @include pading-adnd-aglin();
    @include h1-h2();
}
h1 {
    font-size: 40px;
}

h2 {
    font-size: 35px;
}

h3, h4 {
    @include pading-adnd-aglin();
    @include h3-h4();
}

h3 {
    font-size: 27px;
}

h4 {
    font-size: 20px;
}

</style>