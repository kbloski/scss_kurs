<template>
    <section>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur in similique voluptates quia, vel nobis ipsum quos ducimus minus sunt praesentium culpa deserunt neque perferendis, maxime nostrum voluptatibus necessitatibus quam, veniam cumque dolore saepe exercitationem? Facilis voluptate ab quia eius voluptatum pariatur impedit fugit, provident minus praesentium? Fuga, placeat dicta?</p>
    
        <div class="hyperlinks">
            <p>Przydatne odnoścniki:</p>
            <p><a href="#" id="hyp1"></a></p>
            <p><a href="#" id="hyp2"></a></p>
            <p><a href="#" id="hyp3"></a></p>
            <p><a href="#" id="hyp4"></a></p>
            <p><a href="#" id="hyp5"></a></p>
        </div>
        <a class="more" href="#"></a>
    </section>
</template>

<style lang="scss" scoped>

@function createHyperlinkContent($nr){
    @return 'Link #{$nr}'
}

$hyp-more: 'Pokaż więcej';

#hyp1 {
    &::after {
        content: createHyperlinkContent(1);
    }
}
#hyp2 {
    &::after {
        content: createHyperlinkContent(2);
    }
}
#hyp3 {
    &::after {
        content: createHyperlinkContent(3);
    }
}
#hyp4 {
    &::after {
        content: createHyperlinkContent(4);
    }
}

.more {
    &::after{
        content: $hyp-more;
    }
}

section {
    font-family: Verdana, Geneva, Tahoma, sans-serif;

    .hyperlinks {
        p {
            a{
                color: gray;
                text-decoration: none;
                font-weight: normal;

                &:hover {
                    color: aqua
                }
            }
        }
    }

    a {
        color: green;
        text-decoration: none;
        font-weight: bold;

        &:hover {
            color: #00a000;
        }
    }
}


</style>