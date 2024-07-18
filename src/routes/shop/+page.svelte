<script>
    import filter from '$lib/assets/filter.png';
    import up2 from '$lib/assets/up2.png';
    import tick from '$lib/assets/tick.png';
    import fullstar from '$lib/assets/fullstar.png';
    import halfstar from '$lib/assets/halfstar.png';
    import l1 from '$lib/assets/l1.png';
    import l2 from '$lib/assets/l2.png';
    import l3 from '$lib/assets/l3.png';
    import l4 from '$lib/assets/l4.png';
    import l5 from '$lib/assets/l5.png';
    import l6 from '$lib/assets/l6.png';
    import l7 from '$lib/assets/l7.png';
    import l8 from '$lib/assets/l8.png';
    import l9 from '$lib/assets/l9.png';

    function search() {
        let searchTerm = document.getElementById('find').value.toUpperCase();
        let items = document.querySelectorAll('.product');
        let titles = document.querySelectorAll('.product h2');

        for (let i = 0; i < titles.length; i++) {
            let title = titles[i].innerHTML || titles[i].innerText || titles[i].textContent;
            if (title.toUpperCase().indexOf(searchTerm) > -1) {
                items[i].style.display = "block";
            } else {
                items[i].style.display = "none";
            }
        }
    }
</script>

<div class="px-[100px] min-h-screen">
    <div class="h-px w-[1240px] bg-[#00000010] mb-[40px]"></div>
    <p><a href="/" class="text-[#00000060]">Home&gt;</a> Casual</p>
    <div class="flex mt-[27px]">
        <div class="w-[295px] h-[1220px] rounded-[20px] border border-[#00000010]">
            <div class="flex justify-between pt-[20px] px-[24px] pb-[24px]">
                <h2 class="text-[20px] font-bold">Filters</h2>
                <img src={filter} alt="" class="w-[24px] h-[24px]">
            </div>
            <div class="h-px w-[247px] bg-[#00000010] justify-self-center mx-[24px] mb-[24px]"></div>
            <div class="px-[24px]">
                <div class="flex justify-between">
                    <p class="text-[#00000060] text-[16px]">T-shirts</p>
                    <p class="text-[#00000060] text-[16px]">&gt;</p>
                </div>
                <div class="flex justify-between mt-[20px]">
                    <p class="text-[#00000060] text-[16px]">Shorts</p>
                    <p class="text-[#00000060] text-[16px]">&gt;</p>
                </div>
                <div class="flex justify-between mt-[20px]">
                    <p class="text-[#00000060] text-[16px]">Shirts</p>
                    <p class="text-[#00000060] text-[16px]">&gt;</p>
                </div>
                <div class="flex justify-between mt-[20px]">
                    <p class="text-[#00000060] text-[16px]">Hoodie</p>
                    <p class="text-[#00000060] text-[16px]">&gt;</p>
                </div>
                <div class="flex justify-between mt-[20px]">
                    <p class="text-[#00000060] text-[16px]">Jeans</p>
                    <p class="text-[#00000060] text-[16px]">&gt;</p>
                </div>
            </div>
            <div class="h-px w-[247px] bg-[#00000010] justify-self-center mx-[24px] mt-[24px]"></div>
            <div>
                <div class="flex justify-between pt-[20px] px-[24px] pb-[20px]">
                    <h2 class="text-[20px] font-bold">Colors</h2>
                    <img src={up2} alt="" class="w-[24px] h-[24px]">
                </div>
                <div class="px-[24px] grid grid-cols-5">
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#00C12B] rounded-full mb-[16px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#F50606] rounded-full mb-[16px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#F5DD06] rounded-full mb-[16px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#F57906] rounded-full mb-[16px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#06CAF5] rounded-full mb-[16px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#063AF5] rounded-full relative"><img src={tick} alt="" class="absolute w-[13px] h-[9.5px] top-[10px] left-[10px]"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#7D06F5] rounded-full"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#F506A4] rounded-full"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#FFF] rounded-full"></div>
                    <div class="w-[37px] h-[37px] border-[2px] border-[#00000033] bg-[#000] rounded-full"></div>
                </div>
            </div>
            <div class="h-px w-[247px] bg-[#00000010] justify-self-center mx-[24px] mt-[24px]"></div>
            <div>
                <div class="flex justify-between pt-[20px] px-[24px] pb-[24px]">
                    <h2 class="text-[20px] font-bold">Size</h2>
                    <img src={up2} alt="" class="w-[24px] h-[24px]">
                </div>
                <div class="flex flex-wrap pl-[24px] gap-[8px]">
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">XX-Small</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">X-Small</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">Small</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">Medium</p>
                    <p class="bg-[#000000] px-[20px] py-[10px] rounded-full text-white">Large</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">X-Large</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">XX-Large</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">3X-Large</p>
                    <p class="bg-[#F0F0F0] px-[20px] py-[10px] rounded-full">4X-Large</p>
                </div>
                <p class="mx-[24px] mt-[24px] py-[16px] px-[54px] rounded-full bg-black text-white text-center">Apply Filter</p>
            </div>
        </div>
        <div class="w-auto pl-[20px] mb-[200px]">
            <div class="flex justify-between items-center mb-[18px]">
                <h1 class="font-bold text-[32px]">Casual</h1>
                <p class="text-[16px] text-[#00000060] mr-[24px]">Showing 1-9 of 9 Products</p>
            </div>
            <div class="product-list">
                <div class="flex flex-wrap gap-[20px]">
                    <div class="product">
                        <img src={l1} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Gradient Graphic T-shirt</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                            <p class="text-[14px]">3.5/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <h1 class="font-bold text-[24px]">$145</h1>
                    </div>
                    <div class="product">
                        <img src={l2} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Polo with Tipping Details</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                            <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <h1 class="font-bold text-[24px]">$180</h1>
                    </div>
                    <div class="product">
                        <img src={l3} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Black Striped T-shirt</h2>
                        <div class="flex gap-[5.31px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <p class="text-[14px]">5.0/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <div class="flex gap-2 items-center">
                            <h2 class="font-bold text-[24px] mt-1">$120</h2>
                            <h2 class="font-bold line-through text-[#00000040] text-[24px]">$150</h2>
                            <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-30%</p>
                        </div>
                    </div>
                    <div class="product">
                        <img src={l4} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Skinny Fit Jeans</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                            <p class="text-[14px]">3.5/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <div class="flex gap-2 items-center">
                            <h2 class="font-bold text-[24px] mt-1">$240</h2>
                            <h2 class="font-bold line-through text-[#00000040] text-[24px]">$260</h2>
                            <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-20%</p>
                        </div>
                    </div>
                    <div class="product">
                        <img src={l5} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Checkered Shirt</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                            <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <h1 class="font-bold text-[24px]">$180</h1>
                    </div>
                    <div class="product">
                        <img src={l6} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Sleeve Striped T-shirt</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={halfstar} class="w-[8.79px] h-[16.72px]">
                            <p class="text-[14px]">4.5/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <div class="flex gap-2 items-center">
                            <h2 class="font-bold text-[24px] mt-1">$130</h2>
                            <h2 class="font-bold line-through text-[#00000040] text-[24px]">$160</h2>
                            <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-30%</p>
                        </div>
                    </div>
                    <div class="product">
                        <img src={l7} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Vertical Striped Shirt</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <p class="text-[14px]">5.0/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <div class="flex gap-2 items-center">
                            <h2 class="font-bold text-[24px] mt-1">$212</h2>
                            <h2 class="font-bold line-through text-[#00000040] text-[24px]">$232</h2>
                            <p class="bg-red-100 text-red-600 text-[12px] rounded-full py-[6px] px-[14px]">-20%</p>
                        </div>
                    </div>
                    <div class="product">
                        <img src={l8} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Courage Graphic T-shirt</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <p class="text-[14px]">4.0/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <h1 class="font-bold text-[24px]">$145</h1>
                    </div>
                    <div class="product">
                        <img src={l9} alt="" class="w-[295px] h-[298px]">
                        <h2 class="font-bold text-[20px] mt-[17px]">Loose Fit Bermuda Shorts</h2>
                        <div class="flex gap-[5.31px] mt-[10px] mb-[10.51px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <img src={fullstar} class="w-[18.49px] h-[18.49px]">
                            <p class="text-[14px]">3.0/<span class="text-[#00000060]">5</span></p>
                        </div>
                        <h1 class="font-bold text-[24px]">$80</h1>
                    </div>
                </div>
                <div class="h-px bg-[#00000010] mt-[33px]"></div>
            </div>  
        </div>
    </div>
</div>