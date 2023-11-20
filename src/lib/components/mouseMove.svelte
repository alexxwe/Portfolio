<script lang="ts">
    import { onMount } from 'svelte'
    interface mouseEvent {
        clientX: number
        clientY: number
    }
    interface touchEvent {
        touches: TouchList
    }

    let cards: HTMLDivElement
    let images: NodeListOf<HTMLImageElement>
    let backgrounds: NodeListOf<HTMLDivElement>

    const calcValue = (a: number, b: number): string => ((a / b) * 50 - 50 / 2).toFixed(1)


    onMount(() => {
        const cards = document.querySelector('.cards') as HTMLDivElement

        if (cards) {
            images = cards.querySelectorAll('.card_img_one, .card_img_two, .card_img_three')
            backgrounds = cards.querySelectorAll('.card_bg_one, .card_bg_two, .card_bg_three')

            document.addEventListener('mousemove', (event: mouseEvent) => {
                const yValue = Number(calcValue(event.clientY, window.innerHeight))
                const xValue = Number(calcValue(event.clientX, window.innerWidth))

                cards.style.transform = `rotateX(${yValue}deg) rotateY(${xValue}deg)`

                images.forEach((image: HTMLImageElement) => {
                    image.style.transform = `translateX(${-xValue}px) translateY(${yValue}px)`
                })

                backgrounds.forEach((background: HTMLDivElement) => {
                    background.style.transform = `translateX(${-xValue * 2}px) translateY(${yValue * 2}px)`
                })
            })

            document.addEventListener('touchmove', (event: touchEvent) => {
                const xValue = Number(calcValue(event.touches[0].clientX, window.innerWidth))

                if (xValue >= -50 && xValue <= 50) {
                    cards.style.transform = `rotateY(${xValue}deg)`

                    images.forEach((image: HTMLImageElement) => {
                        image.style.transform = `translateX(${xValue}px)`
                    })

                    backgrounds.forEach((background: HTMLDivElement) => {
                        background.style.transform = `translateX(${xValue * 2}px)`
                    })
                }
            })
        }
    })
</script>

<!-- <div class="flex min-h-screen items-center justify-center overflow-hidden"> -->
<div class="mt-20 flex items-center justify-center xl:h-screen">
    <div bind:this={cards} class="cards">
        <h1 class="text-3xl font-semibold text-indigo-700">Alejandro</h1>
        <h2 class="text-lg">Paz Ferreirós</h2>
        <!-- src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_mono.png" -->
        <div class="card">
            <div class="card_bg_one" />
            <img class="card_img_one" src="/images/finalAlex1.png" alt="" />
            <div class="card_text">
                <p class="card_title">Germany</p>
            </div>
        </div>

        <!-- src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_chihiro.png -->
        <div class="card">
            <div class="card_bg_two" />
            <img class="card_img_two" src="/images/finalAlex2.png" alt="" />
            <div class="card_text">
                <p class="card_title">Milano</p>
            </div>
        </div>

        <!-- src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_howlcastle.png" -->
        <div class="card">
            <div class="card_bg_three" />
            <img class="card_img_three" src="/images/finalAlex3.png" alt="" />
            <div class="card_text">
                <p class="card_title">Prague</p>
            </div>
        </div>
    </div>
</div>

<style>
    h1 {
        text-align: center;
        color: #00b7ff;
        font-size: 30px;
        font-weight: 900;
        /* transform: translateZ(35px); */
    }

    h2 {
        text-align: center;
        color: #ff0000;
        font-size: 20px;
        /* transform: translateZ(25px); */
    }

    .cards {
        /* background: rgb(108, 99, 255); */
        background: transparent;
        border-radius: 20px;
        box-shadow: 0px 10px 20px 20px rgba(0, 0, 0, 0.2);
        display: inline-block;
        padding: 30px 35px;
        min-width: 600px;
        perspective: 1800px;
        transform-style: preserve-3d;
        transform-origin: center;
        /* transform: rotateX(11deg) rotateY(16.5deg); */
    }

    .card {
        border-radius: 15px;
        /* cursor: pointer; */
        display: inline-block;
        height: 300px;
        width: 240px;
        overflow: hidden;
        position: relative;
        text-align: center;
        margin: 0 30px 0 30px;
        box-shadow: 5px 5px 20px -7px rgba(0, 0, 0, 0.5);
        perspective: 1200px;
        transform: translatez(35px);
        transform-style: preserve-3d;
    }

    .card_img_one,
    .card_img_two,
    .card_img_three {
        position: relative;
        height: 100%;
    }

    .card_bg_one,
    .card_bg_two,
    .card_bg_three {
        position: absolute;
        bottom: -50px;
        left: -50px;
        right: -50px;
        top: -50px;
        z-index: 0;
    }

    .card_img_one {
        top: 14px;
        right: -6px;
        height: 110%;
    }
    .card_bg_one {
        /* background: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_monobg.jpg') center / cover no-repeat; */
        background: url('/images/alemaniaPraga.jpg') center / cover no-repeat;
        filter: blur(1px);
    }

    .card_img_two {
        top: 25px;
    }
    .card_bg_two {
        /* background: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_spirited.jpg') center / cover no-repeat; */
        background: url('/images/Finalmilano3.jpg') center / cover no-repeat;
        filter: blur(1px);
    }

    .card_img_three {
        left: 4px;
        height: 110%;
    }
    .card_bg_three {
        /* background: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/62105/3dr_howlbg.jpg') center / cover no-repeat; */
        background: url('/images/praga2.jpg') center / cover no-repeat;
        filter: blur(1px);
    }

    .card_text {
        background: linear-gradient(to bottom, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.637) 100%);
        bottom: 0;
        display: flex;
        height: 70px;
        align-items: center;
        justify-content: center;
        position: absolute;
        width: 100%;
        z-index: 2;
    }

    .card_title {
        color: #fff;
        font-size: 18px;
        font-weight: 700;
    }

    @media (max-width: 768px) {
        .cards {
            /* background: rgb(108, 99, 255); */
            background: transparent;
            border-radius: 20px;
            box-shadow: 0px 10px 20px 20px rgba(0, 0, 0, 0.2);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-width: 300px;
            perspective: 1800px;
            transform-origin: center;
            transform-style: preserve-3d;
        }

        .card {
            border-radius: 15px;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 250px;
            overflow: hidden;
            position: relative;
            width: 175px;
            text-align: center;
            margin: 30px 0 30px 0;
            box-shadow: 5px 5px 20px -7px rgba(0, 0, 0, 0.5);
            perspective: 1200px;
            transform-style: preserve-3d;
            transform: translatez(35px);
        }
    }
</style>
