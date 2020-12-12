### Blog
My personal blog developed using Hugo Static Site Generator and hosted on Netlify.

### How to Run

- Ensure you have installed hugo

```shell
$ sudo pacman -Syy && sudo pacman -S hugo
```
`hugo version`

```
$ ldd --version 
```
```
$ sudo pacman -S glibc
```

- Clone repo.

- Build site + drafts
```
$ make build_all
``` 
- Build site
```
$ make build
```
- Clear Cache
```
$ make clean
```
- View site
Navigate to `http://localhost:1313`

### Credits
* [Hugo Team](https://gohugo.io/)
* [Archie Theme](https://github.com/athul/archie)

## TODO
-