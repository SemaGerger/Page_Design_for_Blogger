<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        list-style: none;
        line-height: 20px;
    }

    body {
        display: grid;
        height: 100vh;
        grid-template-areas: "headerA" "mainA";
        grid-template-rows: 15vh 1fr;
        margin: 0 30px 0 30px;
    }

    .header {
        display: grid;
        grid: "headerA";
        justify-content: center;
    }

    .displayContent {
        display: none;
    }

    /*ana sayfada gözükecek olan ve page'de gözükmeyecek olan i tag'ı*/



    /*! header*/
    .brandName {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 5px;
        background-color: rgb(90, 89, 89);
        border-radius: 10em;
        cursor: default;
    }

    .brandName>h2 {
        color: white;
        text-decoration: underline;
        font-size: 1em;
    }

    .headerMenu {
        display: flex;
        width: auto;
        height: 45px;
        margin: 1em;
        gap: 9px;
        align-items: center;
        justify-content: center;
    }

    .headerMenu>a {
        display: flex;
        width: 28px;
        height: 28px;
        border-radius: 50px;
        box-shadow: 5px 5px 10px #5b5b5b;
    }

    .headerMenu>a:hover {
        height: 30px;
    }

    /*! header end*/



    /*! Content */
    .content {
        display: flex;
        width: fit-content;
        position: relative;
        /*overflow: hidden;*/
        box-shadow: 2px 2px 5px;
        border: 1px dashed rgb(21, 20, 20);
    }

    .contentImg {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
    }

    .main {
        display: grid;
        grid: "mainA";
        gap: 8px;
    }

    .c1 {
        grid-column: span 4;
    }

    .c2 {
        grid-column: span 2;
    }

    .c3 {
        grid-column: span 2;
    }

    .c4 {
        grid-column: span 2;
    }

    .c5 {
        grid-column: span 2;
    }

    .contentWriting {
        grid-column: span 4;
        display: flex;
        justify-content: space-between;
    }

    .contentWriting>h5 {
        padding: 0.3em;
        box-shadow: 2px 2px 5px;
        text-align: center;
        margin: 2% 0 5% 0;
        flex-basis: 23%;
        align-items: center;
    }

    .descriptionHeader {
        grid-column: span 4;
        margin: 0 0 5% 0;
        justify-content: space-between;
    }

    .desc {
        grid-column: span 4;
        column-gap: 40px;
        text-align: justify;
    }


    /*! Content end*/

    /*icons img*/
    .imgAboutIcon {
        background-image: url(https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEifkKHtocl-Ehq82CJwyqvku5nXQDsialY_myv2jU_btj7-ZMP47A5Cle9Y3GIxawkYcbF8j13HWryJoFQ7UQqUbsdiOqeJ7LlmZy4vnhz1y-28_D0IYT8kEDdKnPJ8nixMFrfmLe2EGuwoH75ikiWLcNLyQusVtGB4Of7keXrhb2xmgrVxs7vfM7r1Y_ZO/s1600/about-29-256.png);
    }

    .imgShopIcon {
        background-image: url(https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEi-i43geEBhvu-gdkOFev8sZTD6c9mmxR546RKZ2MNK7IhOKpdqL5eIo47Q563VVf9MNgvd-RnP4HH_pHLvMtpfV1_QgY3SzIVd5B49T8K4IwMk3n4iViwZjKdvhFZf1YMCVEEpkAam0uLMDAq5KHzLc7INNOe-yYAqWlTzVkTjSrde4TErxxgWzeMAiB2r/s320/kisspng-computer-icons-shopping-icon-design-tienda-5b206cc65195a5.2911389015288516543342.png);
    }

    .imgProductIcon {
        background-image: url(https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjKzqHcNRkwbFTUPrKPRG7AKp2fL35xVStCmzvlIajXs-lxjGaZvDhTG-ULK8F2MMzrZhj8UzOUpiNzrrvR6P3NR3iDjq84aDefo09UlXTpKe2m_Gm2Thk7sWp23X9VtKdbK2gWKm3Q-kWsEf0I-TymilYyZ67i_Xpp_nDEqa1c9zPF4qtq-HKtgCBLHVgb/s320/shopping-cart-icon-product-return-shopping-cart-png-32c2d621f780db39d4b1170c31bd1a1e.png);
    }

    .imgIconStyle {
        content: "";
        background-size: cover;
    }

    /*icons img end*/

    /*copyright*/
    .copyright {
        grid-column: span 4;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .savas {
        margin: 10% 0 1% 0;
        font-size: 15px;
    }

    .sema {
        font-size: 9px;
    }

    /*copyright end*/
</style>

<body>
    <!-- for home page view -->
    <i class="displayContent"><img class="contentImg">
        <p id="desc0"></p>
    </i>

    <div class="header headerContent">
        <a class="brandName">
            <h2>THORNY HANDS CRAFT</h2>
        </a>
        <div class="headerMenu">
            <a class="imgAboutIcon imgIconStyle" href="#" target="_blank">
            </a>
            <a class="imgShopIcon imgIconStyle"
                href="https://www.etsy.com/shop/ThornyHandsCraft?ref=l2-about-shopname&listing_id=1569049332"
                target="_blank">
            </a>
            <a class="imgProductIcon imgIconStyle"
                href="https://www.etsy.com/shop/ThornyHandsCraft?ref=l2-about-shopname&listing_id=1569049332"
                id="productLink" target="_blank">
            </a>

        </div>

    </div>

    <div class="main">
        <div class="content c1"><img class="contentImg"></div>
        <div class="content c2"><img class="contentImg"></div>
        <div class="content c3"><img class="contentImg"></div>
        <div class="content c4"><img class="contentImg"></div>

        <div class="content c5"><img class="contentImg"></div>

        <div class="contentWriting">
            <h5>100% Quality</h5>
            <h5>100% Leather</h5>
            <h5>100% HandMade</h5>
            <h5>100% Style</h5>
        </div>
        <div class="descriptionHeader">
            <h2 class="Header"></h2>
            <p class="desc"></p>
        </div>

        <div class="copyright">
            <p class="savas">Product design by Savaş
            <p>
        </div>
        <div class="copyright">
            <p class="sema">@Page design by Sema Gerger
            <p></p>
        </div>
    </div>

    <script>

        var data = {
            images: [
                { src: "https://r.resimlink.com/5pUy9Al.jpeg" },
                { src: "https://r.resimlink.com/kuaxA.jpeg" },
                { src: "https://r.resimlink.com/5pUy9Al.jpeg" },
                { src: "https://r.resimlink.com/4UhmGWpLSRbX.jpeg" },
                { src: "https://r.resimlink.com/_ya0ulWCsR.jpeg" },
                { src: "https://r.resimlink.com/HA42s6_NtD.jpeg" },
            ]
        };


        var hea = "Dark Gray Bracelet";
        var description = ` there any cure for madness? Here is a unique triangle cross necklace for you.
    Pendant, lace, side ornaments, and cord are made of aged genuine black leather.
    Lace's wire is steel
    Pendant's dimensions 5.5cmX4.8cm ,
    Cord's diameter is 2.7mm and full length 65 centimeters.
    The coffin nail and all of the barbed wires are rusty patina. Closure clasp material is 302 ss
    There might be a bit differ patina than pictures because it's handmade patina. So please allow this.
    All of rusty metals parts has been properly cleaned and treated so you can wear safely and comfortably. 
    And the nail fastened tightly by the cross barbed wires.
    `;


        var contentImg = document.querySelectorAll(".contentImg");
        data.images.forEach(function (imageData, index) {
            if (index < contentImg.length) {
                contentImg[index].src = imageData.src;
                contentImg[index].alt = hea;
            }
        });

        function descF() {
            let desc = document.querySelector(".desc");
            desc.textContent = description;
        }
        descF();

    </script>

</body>
