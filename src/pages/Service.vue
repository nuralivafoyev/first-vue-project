<template>
    <section>
        <div class="container">
            <div class="service">
                <div class="service_top">
                    <div class="service_top-txt">
                        <h1>Provide the best service with out of the box ideas</h1>
                        <p>we are a passionate team of digital marketing enthusiasts dedicated to helping businesses
                            succeed
                            in the digital world. With years of experience and a deep understanding of the ever-evolving
                            online landscape, we stay at the forefront of industry trends and technologies.</p>
                    </div>
                    <div class="service_top-cards">
                        <img src="../components/images/service-cards.png" alt="photo">
                        <img class="player" src="../components/images/player.png" alt="photo">
                    </div>
                </div>
                <div class="service_middle">
                    <h1>
                        Real-world examples of how we have helped companies achieve their marketing objectives.
                    </h1>
                    <div class="service_middle-btns">
                        <button>All Work [20]</button>
                        <button>UI/UX Design[10]</button>
                        <button>Digital Marketing [5]</button>
                        <button>Branding [5]</button>
                    </div>
                    <div class="service_middle-cards">
                        <div class="service_middle-cards-card circle">
                            <div class="item">
                                <h1>See Details</h1>
                            </div>
                        </div>

                        <div class="service_middle-cards-card rounded">
                            <h1>
                                <img src="../components/images/vector.png" alt="photo">
                                Ai Corporation. 2023
                            </h1>
                            <p>Ai Wave - Ai Chatbot Mobile App</p>
                        </div>

                        <div class="service_middle-cards-card rounded">
                            <h1>
                                <img src="../components/images/vector.png" alt="photo">
                                Lancer Corporation. 2023
                            </h1>
                            <p>App Lancer - Freelance Mobile</p>
                        </div>
                    </div>

                </div>
                <div class="service_bottom">
                    <div class="service_bottom-txt">
                        <p>“ They thoroughly analyze our industry and target audience, allowing them to develop
                            customized campaigns that effectively reach and engage our customers. Their creative ideas
                            and cutting-edge techniques have helped us stay ahead of the competition.”</p>
                    </div>
                    
                </div>
            </div>
        </div>
    </section>

</template>



<style lang="scss" scoped>
.service {
    padding-top: 70px;
    display: flex;
    align-items: center;
    flex-direction: column;

    &_top {
        gap: 77px;
        display: flex;
        flex-direction: column;

        &-txt {
            display: flex;
            gap: 39px;

            h1 {
                font-size: 48px;
                font-weight: 600;
                color: #010205;
                width: 690px;
            }

            p {
                font-weight: 400;
                color: #878c91;
                width: 557px;
            }
        }

        &-cards {
            position: relative;

            img:hover {
                cursor: pointer;
            }

            .player {
                position: absolute;
                bottom: -15px;
                right: -20px;
                transition: all 0.3s ease;

                &:active {
                    transform: scale(0.96);
                }
            }
        }
    }

    &_middle {
        margin-top: 89px;
        background-color: #020609;
        width: 1408px;
        border-radius: 30px;
        padding: 80px 64px;
        padding-right: 0;

        h1 {
            font-size: 48px;
            font-weight: 600;
            text-align: center;
            margin-bottom: 53px;
            color: #ffffff;
            margin-right: 64px;
        }

        &-btns {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 24px;
            margin-right: 64px;

            button {
                padding: 13px 45.5px;
                border: 1px solid #fff;
                border-radius: 50px;
                background-color: transparent;
                color: #ffffff;
                transition: all 0.3s ease;

                &:hover,
                &:focus {
                    background-color: #99cf63;
                    border-color: #99cf63;
                    color: #010205;
                }
            }
        }

        &-cards {
            display: flex;
            gap: 54px;
            margin-top: 80px;
            position: relative;
            overflow: hidden;

            &-card {
                width: 460px;
                height: 460px;
                border: 11px solid #ffffff66;
                background-color: #c3c3c3;
                border-radius: 50%;

                .item {
                    padding-left: 55px;
                    width: 100%;
                    height: 100%;

                    h1 {
                        background-color: #99cf63;
                        border-radius: 50%;
                        margin-top: 55px;
                        font-size: 18px;
                        font-weight: 700;
                        color: #020609;
                        padding: 70px 35px;
                        text-align: center;
                    }
                }

                &:last-child {
                    position: absolute;
                    right: -178px;
                }
            }

            .circle {
                display: grid;
                place-content: center;

            }

            .rounded {
                border-radius: 30px;
                padding: 32px;
                display: flex;
                flex-direction: column;
                justify-content: space-between;

                h1 {
                    font-size: 17px;
                    font-weight: 600;
                    display: flex;
                    align-items: center;
                    gap: 17px;
                }

                p {
                    font-size: 24px;
                    font-weight: 600;
                    color: #ffffff;
                    line-height: 3px;
                }
            }
        }
    }

    &_bottom {
        &-txt {
            p {
                font-size: 36px;
                font-weight: 600;
                color: #010205;
                margin-top: 115px;
            }
        }
    }
}
</style>