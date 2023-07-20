# Resume

## Quick build
```bash
docker run --rm -v $(pwd):/src klakegg/hugo:0.107.0-ext-alpine --destination=out --minify
docker run --name some-nginx -p 1313:80 -it --rm -v $PWD/out:/usr/share/nginx/html:ro nginx
```

## Quick build

Based on https://themes.gohugo.io/themes/almeida-cv/

```bash
hugo new site resume && cd resume
git submodule add https://github.com/ineesalmeida/almeida-cv.git themes/almeida-cv
```
