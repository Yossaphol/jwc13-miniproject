<script>
    import { onMount } from 'svelte';
    import "./app.css";
    import Trolley from "$lib/assets/trolley.png";
    import Profile from "$lib/assets/profile.png";
    import x from "$lib/assets/x.png";
    import facebook from "$lib/assets/facebook.png";
    import ig from "$lib/assets/instagram.png";
    import github from "$lib/assets/github.png";
    import visa from "$lib/assets/visa.png";
    import master from "$lib/assets/mastercard.png";
    import paypal from "$lib/assets/paypal.png";
    import apple from "$lib/assets/applepay.png";
    import google from "$lib/assets/googlepay.png";


    let isVisible = true;

    onMount(() => {
        const storedState = localStorage.getItem('isVisible');
        isVisible = storedState === null ? true : JSON.parse(storedState);
    });

    function handleClose() {
        isVisible = false;
        localStorage.setItem('isVisible', JSON.stringify(isVisible));
    }
  </script>

{#if isVisible}
<div class="bg-black h-9 flex justify-between items-center">
    <div></div>
    <p class="text-sm text-white">Sign up and get 20% off to your first order. <a href="/" class="underline">Sign Up Now</a></p>

    <div class="message-box">
        <button on:click={handleClose} class="text-white mr-[100px] font-bold">x</button>
    </div>
</div>
{/if}
    <nav class="
flex
flex-row
items-center
justify-center
p-4
bg-white
gap-4
">
    <a href="/" class="font-bold text-3xl mr-4">JWC.CO</a>
    <a href="/shop" class="text-base">Shop</a>
    <a href="/" class="text-base">On Sale</a>
    <a href="/" class="text-base">New Arrivals</a>
    <a href="/" class="text-base">Brands</a>
    <span class="bg-[#F0F0F0] rounded-full flex items-center px-3 cursor-pointer mx-5">
        <svg class="w-[20.27px] h-[20.27px]" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M20.7959 19.2041L16.3437 14.75C17.6787 13.0104 18.3019 10.8282 18.087 8.64606C17.8722 6.46389 16.8353 4.44515 15.1867 2.99936C13.5382 1.55356 11.4014 0.78898 9.20984 0.860705C7.01829 0.932429 4.93607 1.83509 3.38558 3.38558C1.83509 4.93607 0.932429 7.01829 0.860705 9.20984C0.78898 11.4014 1.55356 13.5382 2.99936 15.1867C4.44515 16.8353 6.46389 17.8722 8.64606 18.087C10.8282 18.3019 13.0104 17.6787 14.75 16.3437L19.2059 20.8006C19.3106 20.9053 19.4348 20.9883 19.5715 21.0449C19.7083 21.1015 19.8548 21.1307 20.0028 21.1307C20.1508 21.1307 20.2973 21.1015 20.4341 21.0449C20.5708 20.9883 20.695 20.9053 20.7997 20.8006C20.9043 20.696 20.9873 20.5717 21.044 20.435C21.1006 20.2983 21.1298 20.1517 21.1298 20.0037C21.1298 19.8557 21.1006 19.7092 21.044 19.5725C20.9873 19.4357 20.9043 19.3115 20.7997 19.2069L20.7959 19.2041ZM3.12499 9.49999C3.12499 8.23914 3.49888 7.0066 4.19938 5.95823C4.89987 4.90987 5.89551 4.09277 7.06039 3.61026C8.22527 3.12775 9.50707 3.00151 10.7437 3.24749C11.9803 3.49347 13.1162 4.10063 14.0078 4.99219C14.8994 5.88375 15.5065 7.01966 15.7525 8.25629C15.9985 9.49292 15.8722 10.7747 15.3897 11.9396C14.9072 13.1045 14.0901 14.1001 13.0418 14.8006C11.9934 15.5011 10.7608 15.875 9.49999 15.875C7.80977 15.8733 6.18927 15.201 4.99411 14.0059C3.79894 12.8107 3.12673 11.1902 3.12499 9.49999Z" fill="black" fill-opacity="0.4"/>
            </svg>
            
        <input type="text" placeholder="Search for products..." class="w-[570px] h-12 bg-[#F0F0F0] px-4 py-4 outline-none rounded-full" id="find" on:keyup={search()}>
    </span>
    <div class="flex gap-3 cursor-pointer">
        <img src={Trolley} class="h-6 w-6" />
        <img src={Profile} class="h-6 w-6" />
    </div>
</nav>

<slot />

<footer class="h-[499px] bg-[#F0F0F0] flex flex-col justify-center items-center relative">
    <div class="box bg-black w-[1240px] h-[177px] flex justify-between rounded-[20px] items-center px-[48px] absolute top-[-100px]">
        <div class="w-[45%]">
            <h1 class="text-white text-[40px] font-bold leading-[45px]">STAY UPTO DATE ABOUT OUR LATEST OFFERS</h1>
        </div>
        <div class="flex flex-col items-center justify-center gap-3">
            <span class="bg-[#F0F0F0] rounded-full flex items-center px-3 cursor-pointer mx-5">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M21 4.125H3C2.70163 4.125 2.41548 4.24353 2.2045 4.4545C1.99353 4.66548 1.875 4.95163 1.875 5.25V18C1.875 18.4973 2.07254 18.9742 2.42417 19.3258C2.77581 19.6775 3.25272 19.875 3.75 19.875H20.25C20.7473 19.875 21.2242 19.6775 21.5758 19.3258C21.9275 18.9742 22.125 18.4973 22.125 18V5.25C22.125 4.95163 22.0065 4.66548 21.7955 4.4545C21.5845 4.24353 21.2984 4.125 21 4.125ZM12 11.9738L5.89219 6.375H18.1078L12 11.9738ZM8.69906 12L4.125 16.1925V7.8075L8.69906 12ZM10.3641 13.5262L11.2397 14.3297C11.4472 14.52 11.7185 14.6255 12 14.6255C12.2815 14.6255 12.5528 14.52 12.7603 14.3297L13.6359 13.5262L18.1078 17.625H5.89219L10.3641 13.5262ZM15.3009 12L19.875 7.8075V16.1925L15.3009 12Z" fill="black" fill-opacity="0.4"/>
                    </svg>
                    
                <input type="text" placeholder="Enter your email address" class="w-[300px] h-[48px] bg-[#F0F0F0] px-4 py-4 outline-none rounded-full">
            </span>
            <div class="bg-white w-[349px] px-[16px] py-[12px] rounded-full text-center cursor-pointer">Subscribe to Newsletter</div>
        </div>
    </div>
    <div class="grid grid-cols-5 w-[80%] mt-6" style="display: grid; grid-template-columns: 2fr 1fr 1fr 1fr 1fr; gap: 10px">
        <div>
            <h1 class="font-bold text-[33.45px] mb-3">JWC.CO</h1>
            <p class="text-[#00000060] text-[14px]">We have clothes that suits your style</p>
            <p class="text-[#00000060] text-[14px]">and which you’re proud to wear. </p>
            <p class="text-[#00000060] text-[14px] mb-3">From women to men.</p>
            <div class="flex gap-3">
                <img src={x} class="w-[28px] h-[28px]"/>
                <img src={facebook} class="w-[28px] h-[28px]"/>
                <img src={ig} class="w-[28px] h-[28px]"/>
                <img src={github} class="w-[28px] h-[28px]"/>
            </div>
        </div>
        <div>
            <h2 class="font-medium text-[16px] mb-3">COMPANY</h2>
            <div class="text-[#00000060] flex flex-col gap-2">
                <p>About</p>
                <p>Features</p>
                <p>Works</p>
                <p>Career</p>
            </div>
        </div>
        <div>
            <h2 class="font-medium text-[16px] mb-3">HELP</h2>
            <div class="text-[#00000060] flex flex-col gap-2">
                <p>Customer Support</p>
                <p>Delivery Details</p>
                <p>Terms & Conditions</p>
                <p>Privacy Policy</p>
            </div>
        </div>
        <div>
            <h2 class="font-medium text-[16px] mb-3">FAQ</h2>
            <div class="text-[#00000060] flex flex-col gap-2">
                <p>Account</p>
                <p>Manage Deliveries</p>
                <p>Orders</p>
                <p>Payments</p>
            </div>
        </div>
        <div>
            <h2 class="font-medium text-[16px] mb-3">RESOURCES</h2>
            <div class="text-[#00000060] flex flex-col gap-2">
                <p>Free eBooks</p>
                <p>Development Tutorial</p>
                <p>How to - Blog</p>
                <p>Youtube Playlist</p>
            </div>
        </div>
    </div>
    <div class="h-px w-[1240px] bg-[#00000010] my-[40px]"></div>
    <div class="flex justify-between w-[90%]">
        <p class="text-[#00000060] text-[14px]">JWC.CO © 2000-2023, All Rights Reserved</p>
        <div class="flex gap-4">
            <img src={visa} class="w-[46.61px] h-[30.03px]"/>
            <img src={master} class="w-[46.61px] h-[30.03px]"/>
            <img src={paypal} class="w-[46.61px] h-[30.03px]"/>
            <img src={apple} class="w-[46.61px] h-[30.03px]"/>
            <img src={google} class="w-[46.61px] h-[30.03px]"/>
        </div>
    </div>
</footer>

<!-- <style lang="postcss">
    :global(html) {
      background-color: theme(colors.gray.100);
    }
</style> -->