# django_reset_password
in this repo i will store the django forget password code with full documentation.

## step for create reset password code.
1. go inside setting.py file inside your project Set email backend with smtp crediantails.
note: make sure your app is present in installedapp or static root path  for templates.
```
EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_HOST_USER = 'your email address'
EMAIL_HOST_PASSWORD = 'your password'
EMAIL_USE_TLS = True
DEFAULT_FROM_EMAIL = 'default sending email'

```
2.in app urls.py define path like below.

```
 path('accounts/', include('django.contrib.auth.urls'))
 
 ```
 after defining the path check urls it will look like this.it have lots of urls that provide by django like rest password,login,passord done etc.
 
 - 
![Screenshot (241)](https://user-images.githubusercontent.com/51478832/90765530-bc33a980-e307-11ea-8c27-2e6b1080b6e0.png)


3.After adding urls go inside template and make register folder and place login template there or where you need reset password.
4.add reset password url in your href link in your template like:
```
<a href="{% url "password_reset" %}">&nbsp;&nbsp;Reset password</a>
```
5.now oen the link by click on this button and you will get into reset password page make sure you are using that email that are register with django admin means you are done sign up before reset password.


 
