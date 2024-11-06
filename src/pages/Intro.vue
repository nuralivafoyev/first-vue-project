<template>
    <section id="intro">
        <div class="container">
            <div class="intro_left">
                <div class="intro_left-txt">
                    <strong>Stay ahead of the curve with our forward-thinking </strong>
                    <p>An award-winning SEO agency with disciplines in digital marketing, design, and website development. focused on understanding you.</p>
                </div>
                <div class="intro_left-link">
                    <button>Schedule Call <i class="bi bi-arrow-right"></i></button>
                    <a href="#">View Case Study</a>
                </div>
                <div class="intro_left-brands">
                    <p>Trusted by the world's biggest brands</p>
                    <div class="brands">
                        <img src="../components/icons/afterpay-logo.png" alt="logo"> 
                        <img src="../components/icons/basecamp-logo.png" alt="logo"> 
                        <img src="../components/icons/maze-logo.png" alt="logo"> 
                    </div>
                </div>
            </div>

            <div class="intro_right">
                <img src="../components/images/intro-img.png" alt="img">
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
    #intro {
        padding-top: 153px;
        padding-bottom: 65px;
        .container {
            display: flex;
            justify-content: space-between;
            .intro_left {
                display: flex;
                flex-direction: column;
                gap: 48px;
                &-txt{
                    strong {
                        font-size: 72px;
                        font-weight: 600;
                        color: #010205;
                    }
                    p {
                        color: #878c91;
                        font-weight: 500;
                        margin-top: 48px;
                    }
                }
                &-link{
                    display: flex;
                    gap: 56px;
                    align-items: center;
                    button {
                        background-color: #010205;
                        color: #ffffff;
                        border: 1px solid #010205;
                        padding: 16px 32px;
                        border-radius: 70px;
                        display: flex;
                        gap: 42px;
                        align-items: center;
                        font-weight: 700;
                        transition: all 0.3s ease;
                        &:hover {
                            background-color: transparent;
                            color: #010205;
                        }
                        i {
                            font-size: 24px;
                        }
                    }
                    a {
                        text-decoration: underline;
                        color: #010205;
                        font-weight: 600;
                    }
                }
                &-brands{
                    display: flex;
                    gap: 64px;
                    margin-top: 54px;
                    p {
                        color: #010205;
                        width: 150px;
                        font-weight: 600;
                        font-size: 14px;
                    }
                    .brands {
                        display: flex;
                        gap: 27.93px;
                        img:hover {
                            cursor: pointer;
                        }
                    }

                }
            }

            .intro_right {
                img {
                    animation: animate 4s infinite ease-in-out;
                    &:hover {
                        cursor: pointer;
                    }
                }
            }
        }
    }
    @keyframes animate {
        0% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-20px);
        }
        100% {
            transform: translateY(0);
        }
    }
</style>