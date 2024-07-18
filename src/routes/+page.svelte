<script>
    import './style.css'
    import Head from "$lib/assets/head.png";
    import Ck from '$lib/assets/ck.png';
    import Gucci from '$lib/assets/gucci.png';
    import Prada from '$lib/assets/prada.png';
    import versace from '$lib/assets/versace.png';
    import zara from '$lib/assets/zara.png';
    import star from '$lib/assets/star.png';
    import fullstar from '$lib/assets/fullstar.png';
    import halfstar from '$lib/assets/halfstar.png';
    import t1 from '$lib/assets/t1.png';
    import t2 from '$lib/assets/t2.png';
    import t3 from '$lib/assets/t3.png';
    import t4 from '$lib/assets/t4.png';
    import t5 from '$lib/assets/t5.png';
    import t6 from '$lib/assets/t6.png';
    import t7 from '$lib/assets/t7.png';
    import t8 from '$lib/assets/t8.png';
    import casual from '$lib/assets/casual.png';
    import formal from '$lib/assets/formal.png';
    import party from '$lib/assets/party.png';
    import gym from '$lib/assets/gym.png';
    import ver from '$lib/assets/verify.png';
    import left from '$lib/assets/left.png';
    import right from '$lib/assets/right.png';

    let currentIndex = 0;
    let cards = [
    { 
        id: 1,
        name: 'Sarah M.',
        content: '"I\'m blown away by the quality and style of the clothes I received from JWC.CO. From casual wear to elegant dresses, every piece I\'ve bought has exceeded my expectations.”' 
    },
    { 
        id: 2,
        name: 'Sarah M.',
        content: '"I\'m blown away by the quality and style of the clothes I received from JWC.CO. From casual wear to elegant dresses, every piece I\'ve bought has exceeded my expectations.”' 
    },
    { 
        id: 3,
        name: 'Alex K.',
        content: '"Finding clothes that align with my personal style used to be a challenge until I discovered JWC.CO. The range of options they offer is truly remarkable, catering to a variety of tastes and occasions.”' 
    },
    { 
        id: 4,
        name: 'James L.',
        content: '"As someone who\'s always on the lookout for unique fashion pieces, I\'m thrilled to have stumbled upon JWC.CO. The selection of clothes is not only diverse but also on-point with the latest trends.”' 
    },
    { 
        id: 5, 
        name: 'Mooen',
        content: '"As someone who\'s always on the lookout for unique fashion pieces, I\'m thrilled to have stumbled upon JWC.CO. The selection of clothes is not only diverse but also on-point with the latest trends.”' 
    },
    ]

    const nextCard = () => {
        currentIndex = (currentIndex + 1) % cards.length;
    };

    const prevCard = () => {
        currentIndex = (currentIndex - 1 + cards.length) % cards.length;
    };
</script>

<section class="h-[663px] w-[100%]">
    <img src={Head} class="relative" />
    <div class="w-[40%] absolute top-[160px] left-[100px] translate-x-5 translate-y-5">
        <h1 class="font-bold text-[64px] leading-[64px] mb-[32px]">FIND CLOTHES THAT MATCHES YOUR STYLE</h1>
        <p class="text-[#00000060] text-[16px]">Browse through our diverse range of meticulously crafted garments, </p>
        <p class="text-[#00000060] text-[16px] mb-[31px]">designed to bring out your individuality and cater to your sense of style.</p>
        <a href="/shop" class="py-[16px] px-[54px] text-white bg-black rounded-full ">Shop Now</a>
    </div>
    <div class="flex gap-[32px] absolute top-[540px] left-[100px] translate-x-5 translate-y-5">
        <div class="">
            <h2 class="font-bold text-[40px]">200+</h2>
            <p class="text-[#00000060] font-normal text-base">International Brands</p>
        </div>
        <div class="w-px h-[68px] bg-[#00000010]"></div>
        <div>
            <h2 class="font-bold text-[40px]">2,000+</h2>
            <p class="text-[#00000060] font-normal text-base">High-Quality Products</p>
        </div>
        <div class="w-px h-[68px] bg-[#00000010]"></div>
        <div>
            <h2 class="font-bold text-[40px]">30,000+</h2>
            <p class="text-[#00000060] font-normal text-base">Happy Customers</p>
        </div>
    </div>
    <img src={star} class="absolute right-[120px] top-[220px] w-[104px]"/>
    <img src={star} class="absolute right-[650px] top-[420px] w-[56px]"/>
</section>
<section class="flex overflow-hidden bg-black items-center h-[122px] space-x-16">
    <div class="flex animate-loop-scroll space-x-16" aria-hidden="true">
        <img src={versace} alt="" class="h-[33.16px] max-w-none">
        <img src={zara} alt="" class="h-[37.98px] max-w-none">
        <img src={Gucci} alt="" class="h-[36px] max-w-none">
        <img src={Prada} alt="" class="h-[32px] max-w-none">
        <img src={Ck} alt="" class="h-[33.35px] max-w-none">
    </div>
    <div class="flex animate-loop-scroll space-x-16" aria-hidden="true">
        <img src={versace} alt="" class="h-[33.16px] max-w-none">
        <img src={zara} alt="" class="h-[37.98px] max-w-none">
        <img src={Gucci} alt="" class="h-[36px] max-w-none">
        <img src={Prada} alt="" class="h-[32px] max-w-none">
        <img src={Ck} alt="" class="h-[33.35px] max-w-none">
    </div>
</section>
<section class="flex flex-col justify-center items-center min-h-screen">
    <h1 class="text-[48px] font-bold my-8">NEW ARRIVALS</h1>
    <div class="w-[85%] grid gap-1 grid-cols-4 mb-6">
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t1} />
            </div>
            <h2 class="font-bold text-[20px] my-2">T-shirt with Tape Details</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                    <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <h2 class="font-bold text-[24px] mt-1">$120</h2>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t2} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Skinny Fit Jeans</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                    <p class="text-[14px]">3.5/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <div class="flex gap-2 items-center">
                <h2 class="font-bold text-[24px] mt-1">$240</h2>
                <h2 class="font-bold line-through text-[#00000040] text-[24px]">$260</h2>
                <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-20%</p>
            </div>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t3} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Checkered Sshirt</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                    <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <h2 class="font-bold text-[24px] mt-1">$180</h2>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t4} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Sleeve Stripd T-shirt</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                    <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <div class="flex items-center gap-2">
                <h2 class="font-bold text-[24px] mt-1">$130</h2>
                <h2 class="font-bold line-through text-[#00000040] text-[24px]">$160</h2>
                <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-30%</p>
            </div>
        </div>
    </div>
    <a href="/shop" class="border border-[#00000010] rounded-full px-[54px] py-[16px] w-[218px] text-center">View All</a>
    <div class="h-px w-[1240px] bg-[#00000010] my-[40px]"></div>
    <h1 class="text-[48px] font-bold mb-8">TOP SELLING</h1>
    <div class="w-[85%] grid gap-1 grid-cols-4 mb-6">
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t5} />
            </div>
            <h2 class="font-bold text-[20px] my-2">T-shirt with Tape Details</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <p class="text-[14px]">5.0/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <div class="flex gap-2 items-center">
                <h2 class="font-bold text-[24px] mt-1">$212</h2>
                <h2 class="font-bold line-through text-[#00000040] text-[24px]">$232</h2>
                <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-20%</p>
            </div>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t6} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Skinny Fit Jeans</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <p class="text-[14px]">4.0/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <h2 class="font-bold text-[24px] mt-1">$145</h2>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t7} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Checkered Sshirt</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <p class="text-[14px]">3.0/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <h2 class="font-bold text-[24px] mt-1">$80</h2>
        </div>
        <div>
            <div class="w-[295px] h-[298px] bg-[#F0EEED] rounded-[20px] overflow-hidden">
                <img src={t8} />
            </div>
            <h2 class="font-bold text-[20px] my-2">Sleeve Stripd T-shirt</h2>
            <div class="flex">
                <div class="flex gap-[5.31px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                    <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                    <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                </div>
                <p></p>
            </div>
            <h2 class="font-bold text-[24px] mt-1">$210</h2>
        </div>
    </div>
    <a href="/shop" class="border border-[#00000010] rounded-full px-[54px] py-[16px] w-[218px] text-center my-5">View All</a>
</section>
<section class="flex justify-center items-center my-[36px]">
    <div class="w-[1239px] h-[866px] bg-[#F0F0F0] rounded-[40px] px-[64px] py-[48px]">
        <h1 class="text-center font-bold text-[48px] py-[32px]">BROWSE BY DRESS STYLE</h1>
        <div class="flex flex-wrap gap-4 mt-5">
            <div><img src={casual} alt="" class="w-[407px] h-[289px]"></div>
            <div><img src={formal} alt="" class="h-[289px] w-[684px]"></div>
            <div><img src={party} alt="" class="h-[289px] w-[684px]"></div>
            <div><img src={gym} alt="" class="h-[289px] w-[407px]"></div>
        </div>
    </div>
</section>
<section class="w-full mb-[180px]">
    <div class="pl-[120px] flex justify-between">
        <h1 class="font-bold text-[48px] mb-[38px]">OUR HAPPY CUSTOMERS</h1>
        <div class="control mr-[102px] mt-[36px]">
            <button class="control" on:click={prevCard}><img src={left} alt="" class="w-[20px] h-[20px] mr-[4.12px]"></button>
            <button class="control" on:click={nextCard}><img src={right} alt="" class="w-[24px] h-[24px]"></button>
          </div>
    </div>

    <div class="carousel">
        <div class="cards gap-[10px]" style="transform: translateX(-{currentIndex * 10}%)">
        {#each cards as card (card.id)}
            <div class="card h-[240px] border border-[#00000010] rounded-[20px] px-[32px] py-[28px]">
                <div class="flex gap-[5.31px] mb-[15px]">
                    <img src={fullstar} class="w-[22.58px] h-[22.58px]">
                    <img src={fullstar} class="w-[22.58px] h-[22.58px]">
                    <img src={fullstar} class="w-[22.58px] h-[22.58px]">
                    <img src={fullstar} class="w-[22.58px] h-[22.58px]">
                    <img src={fullstar} class="w-[22.58px] h-[22.58px]">
                </div>
                <div class="flex mb-[12px]">
                    <h3 class="text-[20px] font-bold">{card.name}</h3>
                    <img src={ver} alt="" class="w-[24px] h-[24px]">
                </div>
                <p>{card.content}</p>
            </div>
        {/each}
        </div>
    </div> 
</section>