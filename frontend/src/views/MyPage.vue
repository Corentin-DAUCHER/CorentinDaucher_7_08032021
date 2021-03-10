<!-- TEMPLATE XXX -->

<template>
    
    <div>

        <h1>Bienvenue sur ma page !</h1>

        <h2>Veuillez rentrer un nom d'utilistaeur !</h2>

        <input id="usernameInput" type="text" placeholder="USERNAME">

        <button id="submitButton" type="button">SUBMIT</button>

        <h3>Votre nom d'utilisateur est : <strong id="outputUsername">EMPTY</strong></h3>

    </div>

</template>

<script>

    export default {

        mounted() {

            let username = '';

            const usernameInput = document.getElementById('usernameInput');
            const submitButton = document.getElementById('submitButton');
            const outputUsername = document.getElementById('outputUsername');

            usernameInput.addEventListener('input', function(event) {

                username = event.target.value;

            });

            submitButton.addEventListener('click', function(event) {

                event.stopPropagation();
                console.log('BUTTON CLICKED !')
                console.log(username);

                if(username == ''){

                    username = 'EMPTY';

                }

                outputUsername.innerHTML = username;

            });

        }

    }

</script>
