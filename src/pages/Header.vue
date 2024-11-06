<template>
    <header id="header" :style="{ top: headerTopPosition }">
        <div class="container">
            <div class="header-left">
                <a href="/" class="logo"><img src="../components/icons/logo.png" alt="logo"></a>
                
                <ul>
                    <li><a href="#">Servie</a></li>
                    <li><a href="#">Agency</a></li>
                    <li><a href="#">Case study</a></li>
                    <li><a href="#">Resources</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>

            </div>
            <div class="header-right">
                <button>Get starter</button>
                <a href="#"><img src="../components/icons/bell.svg" alt="img"></a>
            </div>
        </div>
    </header>
</template>

<script>
export default {
  data() {
    return {
      lastScrollTop: 0,  // So'nggi scroll pozitsiyasi
      headerTopPosition: '0px'  // Headerning pozitsiyasi
    };
  },
  mounted() {
    // Scroll eventini Vue komponentiga qo'shamiz
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeDestroy() {
    // Vue komponenti o'chirilganida, eventni to'xtatish
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const currentScroll = window.pageYOffset || document.documentElement.scrollTop;
      
      if (currentScroll > this.lastScrollTop) {
        this.headerTopPosition = '-110px'; 
      } else {
        this.headerTopPosition = '0px';
      }
      this.lastScrollTop = currentScroll <= 0 ? 0 : currentScroll;
    }
  }
};

</script>

<style lang="scss" scoped>
    header {
        transition: all 0.5s ease;
        position: fixed;
        top: 0;
        z-index: 19;
        width: 100%;
        height: 110px;
        background-color: #ffffff8d;
        backdrop-filter: blur(10px);
        display: flex;
        align-items: center;
        justify-content: center;
        .container {
            display: flex;
            justify-content: space-between;
            width: 100%;
            height: 100%;

            .header-left {
                display: flex;
                align-items: center;
                justify-content: space-between;
                gap: 74px;
                .logo {
                    transition: all .3s ease-out;
                    &:hover {
                        transform: rotate(-3deg);
                    }
                }
                ul {
                    display: flex;
                    gap: 33px;
                    li {
                        a {
                            transition: all 0.3s ease;
                            color: #020407;
                            font-size: 14px;
                            font-weight: 600;
                        }
                        &:hover {
                            a {
                                color: #99EA48;
                            }

                        }
                    }
                }
                
            }

            .header-right {
                display: flex;
                align-items: center;
                gap: 9px;
                button {
                    color: #010205;
                    font-size: 14px;
                    font-weight: 700;
                    border: 1px solid #010205;
                    background-color: transparent;
                    border-radius: 50px;
                    padding: 13px 35px;
                    transition: all 0.3s ease;
                    &:hover {
                        background-color: #010205;
                        color: #fff;
                    }
                    &:active {
                        transform: scale(0.96);
                    }
                }
                a {
                    padding: 13px;
                    border-radius: 50%;
                    width: 50px;
                    height: 50px;

                    background-color: #020407;
                    transition: all 0.3s ease;
                    &:hover {
                        color: #99EA48;
                    }
                    &:active {
                        transform: scale(0.96);
                    }
                }
            }
        }
    }
</style>