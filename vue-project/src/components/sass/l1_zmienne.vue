<template>
    <div>
        <h1>Lorem, ipsum dolor.</h1>
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat, culpa
            doloremque. Autem placeat veniam velit odio dolorem accusantium perferendis
            laborum.
        </p>
        <h2>Lorem, ipsum dolor.</h2>
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat, culpa
            doloremque. Autem placeat veniam velit odio dolorem accusantium perferendis
            laborum. Lorem, ipsum dolor.
        </p>
        <h3>Lorem, ipsum dolor.</h3>
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat, culpa
            doloremque. Autem placeat veniam velit odio dolorem accusantium perferendis
            laborum. Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi, illo.
        </p>
    </div>
</template>

<style lang="scss" scoped>
$text-color: #555;
$h1-h6-color: aqua;
$h1-size: 60px;

$p-text-after-size: 1.2rem;
$p-text-after: "Dodany tekst";
$p-text-after-color: green;
$p-text-after-weight: bolder;

// $div-border: 1px solid aqua;
$div-border: 1px solid $h1-h6-color;

h1,h2,h3,h4,h5,h6 {
    color: $h1-h6-color;
}

h1 {
    font-size: $h1-size;
}

p {
    color: $text-color;
}

p:after {
    content: $p-text-after;
    color: $p-text-after-color;
    font-size: $p-text-after-size;
    font-weight: $p-text-after-weight;
}

div {
    border: $div-border;
}


</style>
