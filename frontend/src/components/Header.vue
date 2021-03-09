<!-- TEMPLATE -->

<template>
    
    <div id="header">

        <nav id="navbar">

            <ul>

                <li>

                    <a :href='url1'> {{ text1 }} </a>

                </li>
                
                <li>

                    <a :href='url2'> {{ text2 }} </a>

                </li>

                <li>

                    <a :href='url3'> {{ text3 }} </a>

                </li>

            </ul>

        </nav>

    </div>

</template>

<!-- STYLE -->

<style lang = scss>

    #header{
        width: 100%;
        max-width: 1300px;
        margin: 0px auto;
        display: flex;
        flex-direction: row;
        background-color: lightgrey;

        #navbar{
            width: 100%;
            display: flex;

            ul{
                width: 100%;
                display: flex;
                flex-direction: row;
                justify-content: space-around;

                li{
                    list-style: none;

                    a{
                        text-decoration: none;

                        &:hover{
                            cursor: pointer;
                        }
                        &:visited{
                            color: black;
                        }
                    }
                }
            }
        }
    }

</style>

<!-- SCRIPT -->

<script>

    export default {
        name: 'Header',
        props: ['url1', 'text1', 'url2', 'text2', 'url3', 'text3']
    }

</script>