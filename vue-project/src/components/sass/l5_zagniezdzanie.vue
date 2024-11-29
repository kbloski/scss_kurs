<template>
    <div>Zagniezdzanie</div>

    <div class="top">
        <div class="header">
            <h1>Artykuł 1</h1>
            <p>Podtytuł artukułu <span>1</span></p>
        </div>
    </div>

    <div class="main-content">
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vero quibusdam
            voluptates praesentium fugiat delectus deserunt voluptatibus ex aliquam, odit
            et.
        </p>
        <p class="button">
            <a href="#">Przejdz dalej</a>
        </p>
    </div>
</template>

<style lang="scss" scoped>

@mixin border-subtitle {
    border-bottom: 2px solid #555;;
}

@mixin format {


    .top {
        font-family: 'Verdana';
        margin-top: 50px;

        &:hover {
            filter: blur(2px);
        }

        .header {
            @include border-subtitle;

            h1 {
                text-transform: uppercase;
                color: #666;

                margin-bottom: 0px;
            }

            p {
                font-size: 12px;

                span {
                    font-weight: bold;
                }
            }
        }
    }

    .main-content {
        p {
            font-size: 18px;
            color: rgb(94, 94, 94);
        }

        p.button {
            float: right;

            a {
                text-decoration: none;
                color: black;
                font-weight: bold;
            }
        }
    }
}

@include format; // wywołanie globalne domieszki
</style>
