# Simple Variable List Iterator

Not even sure if the name makes sense, but I hope it makes sense.

Let me know if there is a better tool. Didn't came across so I created this. It works for me, that is all care of.

Works with 1 to `n` variables. If a line is empty, it will add `null` (as in nothing). `[var1]` should be the longest list.

## [Live Demo](https://ittavern.com/svli)

## Examples

```
Template:

Hi, the IP of [var1]'s DNS server is [var2].

-------------------

Variables:

[var1]
Google
Cloudflare

[var2]
8.8.8.8
1.1.1.1

-------------------

Results:
Hi, the IP of Google's DNS server is 8.8.8.8.
Hi, the IP of Cloudflare's DNS server is 1.1.1.1.

```

```
Template:

edit [var4]_[var1]
    set ip [var2] [var3]

-------------------

Variables:

[var1]
app-01
app-02
hr-01

[var2]
10.10.10.15
10.10.10.16
10.10.20.45

[var3]
255.255.255.0
255.255.255.0
255.255.255.0

[var4]
server
server
client

-------------------

Results:

edit server_app-01
    set ip 10.10.10.15 255.255.255.0
edit server_app-02
    set ip 10.10.10.16 255.255.255.0
edit client_hr-01
    set ip 10.10.20.45 255.255.255.0

```

# How-to

Download the `index.html` file, open it in your browser, done. Everything you need in one file.

# TODO

- [ ] License
- [ ] Footer with Git reference + License
- [ ] Save everything temporary to local storage to avoid data loss