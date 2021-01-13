<template>
    <div class="v-header">
        <div class="v-header__brand">
            <button>
                &#9776;
            </button>
            <a href="/e_shop_react">Tennis Shop</a>
        </div>
        <div class="v-header__count">
            <span aria-label="basket" role="img">🛒</span>

        </div>
    </div>
</template>

<script>
    export default {
        name: "v-header"
    }
</script>

<style lang="scss">
    .v-header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 50px;
        padding: var(--spacing-small);
        background-color: #203040;
        //position: fixed;
        top: 0;
        width: 100%;

        &__brand{
            a{
                text-decoration: none;
                font-weight: bold;
                font-size: 1.3rem;
                color: #fff;

                &:hover{
                    color: #ff8000;
                }
            }
            button{
                cursor: pointer;
                font-size: 2rem;
                background: none;
                border: none;
                color: #fff;

                &:hover{
                    color: #ff8000;
                }
            }
        }

        &__count{
            color: #fff;
            margin-left: auto;
            font-weight: bold;
            cursor: pointer;
            padding-right: var(--spacing-small);

            &:hover{
                color: #ff8000;
            }
        }
    }
</style>