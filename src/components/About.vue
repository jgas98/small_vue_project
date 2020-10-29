<template>
 
    <div class = "footer">
 
        <div class = "footer__main">
 
            <div class = "main-col company">
 
                <p class = "text main-text"> Sobre Nosotros </p>
 
                <p class = "text"> Tienda online que trata de vender aparatos electronicos a un precio reducido, disminuyendo su calidad  de manera considerable.</p>
               
            </div>
 
            <div class = "main-col contacts">
 
                <h3 class = "title"> Contacta con nosotros </h3>
 
                <ul class = "footer__list">
 
                    <li class = "footer__list--item"> Galapagar </li>
 
                    <li class = "footer__list--item"> galapagar99@hotmail.com </li>
 
                    <li class = "footer__list--item"> 69834542 </li>
 
                </ul>
 
            </div>
 
        </div>
 
    </div>

</template>

<style lang = "scss">

.footer {margin-top: 24px; width: 100%; background-color: aquamarine;}

.footer__main {
    
    height: auto; width: 100%; display: flex;
    
    justify-content: space-around; flex-flow: row nowrap;
    
    .main-col {width: 30%; padding: 24px;

        .text {font-size: 16px;; font-weight: 300;}

        .main-text {font-weight: 600; font-size: 18px;}
    
    }


    .footer__list {margin-left: -24px; font-size: 16px; 

        .footer__list--item {list-style-type: none;padding: 6px 0;}
    }

}


</style>