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

Create a stronger 20 character password:

```
$ strongpw 20 
wDt!P.6O~}H9vY@`P(2j
```

Create a not so strong password most services will accept:

```
strongpw 20 --no-punctuation
gNQAGzAmxCWj77a4QZI
```

Create very strong passwords for 500 "friends" on social media.

```
strongpw -r 500 -l 30
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
