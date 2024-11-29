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
// Importowanie plików scss
@import './variables.scss';
@import './mixins.scss';



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