# UCMS v.1.5.0 Information leakage

> A problem was found in UCMS 1.5.0. In line 2 of ucms/top.php

## Vulnerability Type :

Information leakage



## Vulnerability Version :

1.5.0

## Vulnerability Description:

> ucms/top.php:2

![image-20210111163037671](C:\Users\grq\AppData\Roaming\Typora\typora-user-images\image-20210111163037671.png)

1.There is no adminchannelscache() defined in top.php, it will  report an  error when directly accessing top.php

2.ucms/top.php can be accessed directly by anyone.  adminchannelscache() will report an  error, so that the current physical path is revealed



## Recurring environment:

- Windows 10
- PHP 5.4.5
- Apache 2.4.23

## Vulnerability recurrence:

![image-20210111162943065](C:\Users\grq\AppData\Roaming\Typora\typora-user-images\image-20210111162943065.png)
