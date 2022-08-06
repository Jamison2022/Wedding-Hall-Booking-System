# WHBS-XSS

The Wedding Hall Booking System published in SourceCodester has multiple Cross-site scripting vulnerabilities. The system does not do anything with input and output. Attackers can construct malicious code to steal user and administrator cookies.



## Contact Us

```
/whbs/?page=contact_us
```

![image-20220806143046818](WHBS-XSS.assets/image-20220806143046818.png)

![image-20220806143236190](WHBS-XSS.assets/image-20220806143236190.png)





## Booking Form

![image-20220806143701212](WHBS-XSS.assets/image-20220806143701212.png)

Fires when the user views the booking

```
/whbs/?page=my_bookings
```

![image-20220806143829185](WHBS-XSS.assets/image-20220806143829185.png)

Fires when the admin views the booking

```
/whbs/admin/?page=bookings
```

![image-20220806144106420](WHBS-XSS.assets/image-20220806144106420.png)



## Profile page

Modify the profile

```
/whbs/?page=manage_account
```

![image-20220806144716946](WHBS-XSS.assets/image-20220806144716946.png)

Fires when the user views the profile

```
/whbs/?page=profile
```

![image-20220806145124839](WHBS-XSS.assets/image-20220806145124839.png)

Fires when the admin views the Client Lists

```
/whbs/admin/?page=clients
```

![image-20220806145620104](WHBS-XSS.assets/image-20220806145620104.png)







## Staff user profile

```
/whbs/admin/?page=user
```

![image-20220806151214286](WHBS-XSS.assets/image-20220806151214286.png)

Fired when an administrator visits the User List page.

```
/whbs/admin/?page=user/list
```

![image-20220806151352449](WHBS-XSS.assets/image-20220806151352449.png)

All of the above vulnerabilities can return cookies.



## Link

https://www.sourcecodester.com/php/15154/wedding-hall-booking-system-phpoop-free-source-code.html