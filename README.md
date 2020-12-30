# strongpw
Helper script to create strong passwords. 

Default minimum length are 12 characters based on

```
abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
0123456789
!" #$%&\'()*+,-./:;<=>?@[\\]^_`{|}~
```

## Example

Create a strong password with a default length of 12 characters.

```
$ strongpw
Eisv&<*U\] B
```

Same, but disallow certain characters, e.g. space, asterisk and plus:

```
$ strongpw -d ' *+'
&'wZ4PtRh&SC
```


Create a stronger 20 character password:

```
$ strongpw 20 
wDt!P.6O~}H9vY@`P(2j
```

Create a not so strong password most services will accept:

```
$ strongpw 20 --no-punctuation
gNQAGzAmxCWj77a4QZI
```

Same but verify the generated password has not been pwned as far as the haveibeenpwned service can tell:

```
$ strongpw --no-punctuation --check-pwned -l 20
lTRJdsCIXm7YZq26PWRO
```

Create a given number of passwords with a defined length:

```
$ strongpw -r 20 -l 16
QFEB.*t\![ncvtH`WN{]Jy?"`I(Cbk
b#x<P"m2Mpx7c@9?}.7y/'#l`m9aAO
p" :JweaLkeg"B DX^Hn(eLzA^%mSR
WJG<to,HQ^T9Fx!>mq.`/yC' bh+8+
}!vy<M#0WjM\4u3:;6eMD=~5`K=]<~
Di^\-{<U=h%n0]DM/'le6b8nQkSU;1
o]~}S{!*l:rKmfZIuw5UOrg:-&prmu
<QUR`YcY"d1yVe'#\S$&2ULkWs Fp{
h)!JhEL.dU%oOsH`F (iv:\M`*v4O_
!!wt1G~.UW%[j2YY-X@S-N|0zpl?F*
...
```

Create a password based on a given alphabet (target):

```
$ strongpw -t hosteurope_ssh
h62pn;WGNpm^
```

This is currently rather an implementation idea as alphabets for passwords should usually not be restricted. Might be rather rare nower days.

List the available targets:

```
$ strongpw --list-targets
hosteurope_ssh
test_weak_alphabet
```
