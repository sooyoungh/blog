# Blog

<aside>
  
    ๐ Web Architecture๋ฅผ ๊ณต๋ถํ๊ธฐ ์ํด ๊ตฌํํ ๋ธ๋ก๊ทธ(๊ฒ์ํ) ํ๋ก์ ํธ

</aside>

  1. [JSP + Servlet](#ver1-jsp--servlet)
  2. [JSP + Spring MVC](#ver2-jsp--spring-mvc)
  3. [Front + Back(Spring Boot)](#ver3-front--backspring-boot)


## ver1. JSP + Servlet

![image](https://user-images.githubusercontent.com/77563814/191008015-aa4aa778-db29-4446-b2e1-84c033afc29f.png)



<aside>
  
    โ๏ธ ๊ฐ์ฅ ๋จ์ํ MVC2 ํจํด์ผ๋ก, M,V,C๊ฐ ๋ถ๋ฆฌ๋์ด ์๋ค.

</aside>

- Jsp (View)
- Servlet (Controller)
- JavaBeans (Model)

> ๋์ ๊ณผ์ 
> 
>     1. ์๋ธ๋ฆฟ(Controller)์ด ์์ฒญ์ ๋ฐ๋๋ค. 
>     2. ์๋ฐ ๋น(Model)์ด ๋น์ฆ๋์ค ๋ก์ง ์ฒ๋ฆฌ ํ, ๋ทฐ(jsp)์ ๋ฐํํ๋ค. 
>     3. ๋ทฐ(jsp)๋ ๊ฒฐ๊ณผ๋ฅผ ์ ๋ฌ๋ฐ์ ์ต์ข ํ๋ฉด์ ์ถ๋ ฅํ๋ค.


## ver2. JSP + Spring MVC
![image](https://user-images.githubusercontent.com/77563814/191040036-9f5dac4f-322a-46e5-906a-cc54debd93ee.png)

<aside>
  
    โ๏ธ ๋ชจ๋  ์์ฒญ/์๋ต์ ๋ฐ๋ FrontController์ ๋์ํ Spring MVC ๊ตฌ์กฐ๋ก, 
        FrontController๊ฐ Controller/View๋ฅผ ์ฐพ์ ์์ฒญ/๋ฐํ์ ๋ด๋นํ๋ค.

</aside>

- Jsp (View)
- Spring Framework (Controller + Model)
    - Controller
    - Service
    - Dao

> ๋์ ๊ณผ์ 
> 
>     1. ๋ชจ๋  ์์ฒญ์ Front Controller(Dispatcher-Servlet)์ด ๋ฐ์์ ํด๋นํ๋ Controller๋ฅผ ์ฐพ๋๋ค. 
>     2. ํด๋น ์์ฒญ์ ๋ฐ๋ฅธ ๋น์ฆ๋์ค ๋ก์ง ์ฒ๋ฆฌ ํ Front Controller์ ๋ฐํํ๋ค.
>     3. ํด๋นํ๋ ๋ทฐ(jsp)๋ฅผ ์ฐพ์ Front Controller์ ๋ฐํ, ์ต์ข ์ถ๋ ฅํ๋ค.



## ver3. Front + Back(Spring Boot)
![image](https://user-images.githubusercontent.com/77563814/191008041-991b8d92-a3b1-48e0-b686-6869213c6358.png)


<aside>

    โ๏ธ ํ๋ก๊ทธ๋จ์ด ํ์ฅ๋จ์ ๋ฐ๋ผ ํ๋ก ํธ์ ๋ฐฑ์๋๋ฅผ ๋ถ๋ฆฌํ ์น ๊ตฌ์กฐ๋ก, 
        ์๋ก Http ํต์ ํ์ฌ jsonํํ๋ก ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ  ๋ฐ๋๋ค.

</aside>




- Front : Html, Css, Javascript
- Back : Spring Boot


> ๋์ ๊ณผ์ 
> 
>     1. ํ๋ก ํธ์์ ์์ฒญ์ ๋ฐ์ผ๋ฉด Ajax ํต์ ์ผ๋ก ๋ฐฑ์ ์ ๋ฌํ๋ค. 
>     2. ๋ฐฑ์์ Controller-Service-Repository ๊ณ์ธต ๊ฐ๊ฐ์ ๋ง๊ฒ ๋ก์ง ์ฒ๋ฆฌํ๊ณ  ๊ฒฐ๊ณผ๋ฅผ ํ๋ก ํธ์ ๋ฐํํ๋ค.
>     3. ํ๋ก ํธ์์ ํด๋น ๊ฒฐ๊ณผ๋ฅผ ํ ๋๋ก ๋ทฐ(Html)๋ฅผ ์ถ๋ ฅํ๋ค.

