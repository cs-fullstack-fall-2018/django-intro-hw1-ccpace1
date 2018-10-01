# django-intro-hw1

Create a new route and paste it below. Create a blue-or-red route that takes an argument of blue or red. If it's blue, write "Sky". If it's red, write "Fire". If it's anything else write "ERROR".

Route: 
    path('<str:redorblue>/', views.redOrBlue)

Code:
    def redOrBlue(request, redorblue):
    
    if (redorblue=='blue'):
        return HttpResponse("SKY")
    elif (redorblue=='red'):
        return HttpResponse("Fire")
    else:
        return HttpResponse("ERROR")
