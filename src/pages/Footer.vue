<template>
    <footer>
        <div class="container">
            <div class="footer_card">
                <h1>Ready to work with us ?</h1>
                <button>Get Started <i class="bi bi-arrow-right"></i></button>
            </div>
            <div class="wrapper">

                <div class="social_media">
                    <div class="social_media-socials">
                        <a href="/" class="logo"><img src="../components/icons/logo.png" alt="logo"></a>
                        <p>We offers a comprehensive suite of digital marketing services that cover all aspects of our
                            online presence. From SEO and social media marketing to content creation and PPC
                            advertising,
                            they have the expertise and resources to handle our diverse marketing needs.</p>
                        <div class="social_media-socials-wrapper">
                            <i class="bi bi-facebook"></i>
                            <i class="bi bi-twitter"></i>
                            <i class="bi bi-linkedin"></i>
                            <i class="bi bi-instagram"></i>
                        </div>
                    </div>
                </div>

                <nav class="navs">
                    <ul>
                        <h1>Navigation</h1>
                        <li><a href="#">Service</a></li>
                        <li><a href="#">Agency</a></li>
                        <li><a href="#">Case Study</a></li>
                        <li><a href="#">Resource</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                    <ul>
                        <h1>Licence</h1>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Copyright</a></li>
                        <li><a href="#">Email Addres</a></li>
                    </ul>
                    <ul>
                        <h1>Contact</h1>
                        <li><a href="#"><i class="bi bi-telephone-fill"></i> (406) 555-0120</a></li>
                        <li><a href="#"><i class="bi bi-envelope-fill"></i> Hey@boostim.com</a></li>
                        <li><a href="#"><i class="bi bi-geo-alt-fill"></i> 2972 Westheimer Rd. Santa Ana, Illinois 85486 </a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    width: 100%;
    padding-top: 120px;

    .footer_card {
        width: 1408px;
        background-color: #020609;
        transform: translateX(-64px);
        border-radius: 30px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 81px 64px;

        h1 {
            color: #fff;
            font-size: 80px;
            font-weight: 600;
        }

        button {
            background-color: #fff;
            color: #020609;
            border: 1px solid #fff;
            border-radius: 70px;
            font-size: 16px;
            padding: 16px 32px;
            display: flex;
            gap: 42px;
            transition: all 0.3s ease;

            &:hover {
                background-color: #020609;
                color: #fff;
            }
        }
    }

    .wrapper {
        display: flex;
        margin-top: 84px;
        gap: 108px;
        .social_media {
            display: flex;
            justify-content: space-between;

            &-socials {
                display: flex;
                flex-direction: column;
                align-items: start;
                gap: 30px;

                .logo {
                    transition: all .3s ease-out;

                    &:hover {
                        transform: rotate(-3deg);
                    }
                }

                p {
                    font-size: 14px;
                    font-weight: 400;
                    color: #9B9B9C;
                    width: 534px;
                }

                &-wrapper {
                    display: flex;
                    gap: 16px;
                    align-items: center;
                    color: #020609;

                    i {
                        width: 34px;
                        height: 34px;
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        text-align: center;
                        padding: 8px;
                        background-color: #fff;
                        border-radius: 50%;
                        cursor: pointer;
                    }
                }
            }
        }

        .navs {
            display: flex;
            justify-content: space-between;
            width: 100%;
            ul {
                display: flex;
                flex-direction: column;
                align-items: start;
                gap: 15px;
                h1 {
                    margin-bottom: 40px;
                }
                li {
                    a {
                        color: #9B9B9C;
                        font-size: 14px;
                    }
                }
            }
        }
    }
}
</style>