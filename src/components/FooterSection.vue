<template>
    <div class="footer">
        <div class="flex-between">
            <div class="first-column">
                <div>
                    <div class="flex">
                        <img class="logo" src="@/assets/images/logo_light.png" alt="Logo footer">
                        <h4 style="margin-left: 10px; font-size: 24px;">Source?</h4>
                    </div>
                    <p style="margin-top: 14px; line-height: 1rem;">Source est une extension web de Twitter qui vous permettra de vérifier le contenu d’un tweet à l’aide d’un système de fiabilité de l’information qui n’a jamais été aussi objectif.</p>
                </div>
                <div style="margin-top: 50px;">
                    <h4>Nous contacter</h4>
                    <p style="margin: 14px 0; line-height: 1rem;">N’hésitez pas à nous envoyer un mail si vous avez la moindre question !</p>
                    <a href="">support@source.com</a>
                </div>
            </div>
            <div class="second-column">
                <div class="flex-between">
                    <div>
                        <h4>À propos</h4>
                        <ul>
                            <li>
                                <a href="">Accueil</a>
                            </li>
                            <li>
                                <a href="">Qui sommes nous ?</a>
                            </li>
                            <li>
                                <a href="">FAQs</a>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h4>Nous suivre</h4>
                        <ul>
                            <li>
                                <a href="">Twitter</a>
                            </li>
                            <li>
                                <a href="">Facebook</a>
                            </li>
                            <li>
                                <a href="">Discord</a>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h4>À propos</h4>
                        <ul>
                            <li>
                                <a href="">FAQs</a>
                            </li>
                            <li>
                                <a href="">Installation</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="divider"></div>
                <div class="flex">
                    <p style="font-weight: 500; font-size: 18px;">Ajoutez l’extension Source? à votre navigateur et à votre compte Twitter</p>
                    <button>Ajouter à Chrome</button>
                </div>
            </div>
        </div>
        <div class="flex-between footer_bar">
            <p>©2022 Source?</p>
            <div>
                <a href="">CGU</a>
                <a href="">Mentions légales</a>
                <a href="">Cookies</a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    .footer {
        padding: 72px $margin-width;
        background-color: #000;
        color: #fff;
        font-size: 14px;

        &_bar {
            margin-top: 70px;

            div a {
                text-decoration: none;
                font-weight: 400;
                display: inline-block;
                margin-left: 80px;
            }
        }

        a {
            color: #fff;
            font-weight: bold;
        }

        h4 {
            margin-bottom: 14px;
        }

        li {
            margin-bottom: 8px;

            a {
                text-decoration: none;
                font-weight: normal;
            }
        }
    } 

    .flex {
        display: flex;
        align-items: baseline;
    }

    .flex-between {
        display: flex;
        justify-content: space-between;
    }
    
    .logo {
        width: 43px;
        height: 41.9px;
    }

    .first-column {
        width: 42%;
    }

    .second-column {
        width: 50%;
    }

    .divider {
        height: 1px;
        width: 100%;
        background-color: #fff;
        margin: 70px 0 40px;
    }
</style>