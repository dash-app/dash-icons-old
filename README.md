Dash-App Icons
===============================

## How to Export

### with docker
```bash
docker run --rm --name exports-fonts \
    -v $PWD:/work --workdir="/work" --entrypoint=npx \
    -it node icon-font-generator ./SVG/*.svg -o ./fonts/ --name="dh-icon" --height 100
```

### without docker
```bash
npx icon-font-generator ./SVG/*.svg -o ./fonts/ --name="dh-icon" --height 100
```
