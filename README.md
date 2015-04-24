# strongpw
Helper script to create strong passwords.

## Example

Create a strong 20 character password:

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
