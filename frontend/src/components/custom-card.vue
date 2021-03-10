<template>
    
    <div class="card">

        <slot name="title">

            <h3>Titre de la carte</h3>

        </slot>

        <slot name="text">

            <h3>Texte de la carte</h3>

        </slot>

        <slot name="action">

            <button>Action</button>

        </slot>

    </div>

</template>

<style lang="scss" scoped>

    .card {
        width: 100%;
        max-width: 400px;
        margin: 0px auto;
        padding: 20px;
        background-color: lightgrey;
    }

</style>

<script>

    export default {

        name: 'Card'

    }

</script>
