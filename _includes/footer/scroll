/* Scroll to top */
jQuery(document).ready(function(){
  jQuery('nav ul li a').click(function(){
    var el = jQuery(this).attr('href');
    var elWrapped = jQuery(el);

    scrollToDiv(elWrapped,40);		
    return false;	
  });
	
  function scrollToDiv(element,navheight){
    var offset = element.offset();
    var offsetTop = offset.top;
    var totalScroll = offsetTop-navheight;
		
    jQuery('body,html').animate({
      scrollTop: totalScroll
    }, 500);
  }
});

/* Show/Hide back to top button */
jQuery(document).ready(function(){
  jQuery(window).scroll(function(){
    if (jQuery(this).scrollTop() > 200) {
      jQuery('.go-top').fadeIn(300);
    } else {
      jQuery('.go-top').fadeOut(300);
    }
  });

  jQuery('.go-top').click(function(event){
    event.preventDefault();
    jQuery('html, body').animate({
      scrollTop: 0
    }, 300);
  });
});
