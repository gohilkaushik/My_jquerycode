# My_jquerycode

// Accordin js
$('.accordin-title').click(function(e){
    e.preventDefault();
    const accordinTitle = $(this).closest('.accordin-title');
    accordinTitle.next().toggleClass('show');

    const icon = accordinTitle.find("i");
    if(icon.hasClass("fa-plus-circle")){
        icon.removeClass('fa-plus-circle');
        icon.addClass('fa-minus-circle')
    }
    else if(icon.hasClass("fa-minus-circle")){
        icon.addClass('fa-plus-circle');
        icon.removeClass('fa-minus-circle')
    };
})
