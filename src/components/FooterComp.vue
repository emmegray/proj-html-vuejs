<template>
    <nav>
        <div class="footer bg-ebony-clay">
            <img src="/img/logo_footer.png" class="logo" alt="logo">
            <ul>
                <li>
                    <a href="#">Home</a>
                </li>
                <li>
                    <a href="#">Meet The Brand</a>
                </li>
                <li>
                    <a href="#">Live Dates</a>
                </li>
                <li>
                    <a href="#">Lates News</a>
                </li>
                <li>
                    <a href="#">Albums</a>
                </li>
                <li>
                    <a href="#">Fans</a>
                </li>
            </ul>
        </div>
        <div class="copyright bg-charade">
            <div>
                <span>&#169; Copyright 2021 - 2020</span> | <span>Avada theme by themefusion</span> | <span>all rights
                    reserved</span> | <span>powered by wordpress</span>
            </div>
            <div>
                <ul class="social">
                    <li>
                        <a href="#">
                            <font-awesome-icon icon="fa-brands fa-facebook-f" />
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <font-awesome-icon icon="fa-brands fa-twitter" />
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <font-awesome-icon icon="fa-brands fa-instagram" />
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <font-awesome-icon icon="fa-brands fa-youtube" />
                        </a>
                    </li>
                </ul>
                <button>
                    <a href="#">
                        <font-awesome-icon icon="fa-solid fa-chevron-up" />
                    </a>
                </button>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'FooterComp'
}
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

.footer {
    width: 100%;
    height: 90px;
    padding: 0px 20px 0px 20px;
    text-align: start;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    z-index: 1000;
}

ul {
    margin: 0;
    padding: 0;
}

ul,
li {
    display: inline-block;
    margin-right: 15px;
    font-size: small;
}

a {
    color: $mid-gray;
    text-decoration: none;

    &:hover {
        color: $white;
    }
}

.copyright {
    @extend .footer;
    font-size: x-small;
    color: $mid-gray;
    position: relative;

    span:not(:first-child) {
        text-transform: uppercase;
    }
}

.social li {
    display: inline-flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    height: 37px;
    width: 37px;
    background: $ebony-clay;
}

button {
    position: absolute;
    bottom: 0;
    right: 15px;
    color: $white;
    background: #323233;
    padding: 5px 10px;
    border: 0;

    a {
        color: $white;
    }
}
</style>