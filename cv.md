# _Shishlo Andrey_

![My photo](../rsschool-cv/assets/img/myphoto.jpg)

student in RS-School

## **My сontacts:**

- **Phone:** +375-25-521-31-63
- **Email:** shishlik19@gmail.com
- **Telegram:** @andreyshishlo
- **Instagram:** i_andreyshishlo
- **GitHub:** AndreySh1
- **Discord:** AndreyShishlo(AndreySh1)

## **About me**

I'm 30 years old. Having started his career, I had to try myself in various fields of activity, where often no intellectual development was expected.
My goal is to make my life better and more interesting. I want to grow, develop my skills and make new acquaintances. For this reason, I chose Front-End development.
I've been studying web development for about 2 years. Several Front-End Developer courses have been completed and several trial projects have been completed.
My dedication and sociability will help me grow and develop in my chosen profession.

## **My skills**

Basic knowledge:

- HTML, CSS
- JavaScript

## **Code examples**

**_for the presentation site of the new ASUS model:_**

```
var videoA = function () {this.innerHTML = '<iframe width="660" height="415" src="https://www.youtube.com/embed/qHQVjfpz6nE"
title="YouTube video player" frameborder="0" allow="accelerometer; autoplay;
clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>'};
document.querySelector('.video-center').addEventListener('click', function (e) { this.removeEventListener('click', videoA, false);
videoA.apply(this, arguments); } , false);
```

**_for the presentation site of the new TESLA model:_**

```
  $(document).scroll(function() {
	if($(document).scrollTop()>200)
	{
		/*$(".header-t").css('padding','1px 0 1px 15px').css('background','red');*/
		$(".header-t").css('padding','1px 0 1px 5px');
		$(".head-0").css('background','#333');
		$("#logo").attr('src','images/tesla-logo3.png');

	}
	if($(document).scrollTop()<=200)
	{
		$(".header-t").css('padding','15px 0 10px 20px');
		$(".head-0").css('background',' rgba(7,7,7,0.3)');
		$("#logo").attr('src','images/tesla-logo1.png');
	}
})

  $('#at').hover(function(){
	$(this).attr('src','images/video-play-bl.png');},
	function(){
	$(this).attr('src','images/video-play.png');
	});
```

**_for a site using the API:_**

```
const input = document.getElementById('input');
const grid = document.getElementsByClassName('grid')[0];

document.getElementById('input').focus();

window.onload = function() {
    loadImg1();
  };

async function loadImg1 (){
    const urlTesla = 'https://api.unsplash.com/search/photos?query=tesla&per_page=20&orientation=landscape&client_id=cWNhoJw52_EtPg8bqwun-XsMBG-uUi3TVBSet2KhF7g';
    fetch(urlTesla)

    .then(response =>{
        if(response.ok)
        return response.json();
        else
        alert(response.status)
    })

    .then(data => {
        const imageNodes = [];
        for(let i = 0; i < data.results.length;i++){
            imageNodes[i] = document.createElement('div');
            imageNodes[i].className = 'img';
            imageNodes[i].style.backgroundImage = 'url(' +data.results[i].urls.raw+')';
            imageNodes[i].addEventListener('dblclick',function(){
                window.open(data.results[i].links.download, '_blank');
            })
            grid.appendChild(imageNodes[i]);
        }
    })
}



input.addEventListener('keydown', function(event){
    if(event.key === 'Enter' && (input.value !== ''))
    loadImg();
    if(event.key === 'Enter' && (input.value == ''))
    loadImg1();
})

function loadImg(){
    removeImages();

    const url = 'https://api.unsplash.com/search/photos/?query='+input.value+'&per_page=30&client_id=cWNhoJw52_EtPg8bqwun-XsMBG-uUi3TVBSet2KhF7g';
    fetch(url)

    .then(response =>{
        if(response.ok)
        return response.json();
        else
        alert(response.status)
    })

    .then(data => {
        const imageNodes = [];
        for(let i = 0; i < data.results.length;i++){
            imageNodes[i] = document.createElement('div');
            imageNodes[i].className = 'img';
            imageNodes[i].style.backgroundImage = 'url(' +data.results[i].urls.raw+')';
            imageNodes[i].addEventListener('dblclick',function(){
                window.open(data.results[i].links.download, '_blank');
            })
            grid.appendChild(imageNodes[i]);
        }
    })
}

function removeImages(){
    grid.innerHTML = '';
}
```

## **Experience**

- [Kursy.by](Kursy.by)
- [FructCode](fructcode.com)

## **Education**

- 2020

  - online training at [IT-KAMASUTRA](https://www.youtube.com/c/ITKAMASUTRA).
  - online training at [FructCode](https://fructcode.com/ru/).

- 2021

  - Completed the Front-End developer course at KURSY.BY.

- 2021-2022

  - student in RS-School

  ## **English**

My English level is basic (A1-A2). Started learning the language on the platform [Duolingo](https://ru.duolingo.com) . I intend to improve my level up to C2-Proficiency.
