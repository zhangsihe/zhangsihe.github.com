
    $('.scroll_top').click(function(){$('html,body').animate({scrollTop: '0px'}, 800);});     //页面滚动至顶部

    $('.scroll_a').click(function(){$('html,body').animate({scrollTop:$('.a').offset().top}, 800);});    //页面滚动至指定的位置

    $('.scroll_bottom').click(function(){$('html,body').animate({scrollTop:$('.bottom').offset().top}, 800);});   //页面滚动到底部