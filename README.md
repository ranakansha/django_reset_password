# django_reset_password
in this repo i will store the django forget password code with full documentation.

##step for create reset password code.
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
 after defining the path check urls it will look like this
 
