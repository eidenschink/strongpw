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
```

Create a stronger 20 character password:

```
$ strongpw 20 
```

Create a not so strong password most services will accept:

```
strongpw 20 --no-punctuation
```

Create very strong passwords for 500 "friends" on social media.

```
strongpw -r 500 -l 30
```
