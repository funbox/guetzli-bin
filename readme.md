# guetzli-bin ![GitHub Actions Status](https://github.com/imagemin/guetzli-bin/workflows/test/badge.svg?branch=main)

> [Guetzli](https://github.com/google/guetzli) is a JPEG encoder that aims for excellent compression density at high visual quality. Guetzli-generated images are typically 20-30% smaller than images of equivalent quality generated by libjpeg.

You probably want [`imagemin-guetzli`](https://github.com/imagemin/imagemin-guetzli) instead.

**Note! This is a fork of [guetzli-bin](https://github.com/imagemin/guetzli-bin) repo that we need to make [Optimizt](https://github.com/funbox/optimizt) work [right](https://github.com/funbox/optimizt/issues/48). The fork will probably be removed after [guetzli-bin#18](https://github.com/imagemin/guetzli-bin/pull/18) merge.**


## Install

```
$ npm install guetzli
```


## Usage

```js
import {execFile} from 'node:child_process';
import guetzli from 'guetzli';

execFile(guetzli, ['input.jpg', 'output.jpg'], error => {
	console.log('Image minified!');
});
```


## CLI

```
$ npm install --global guetzli
```

```
$ guetzli --help
```


## License

MIT © [Imagemin](https://github.com/imagemin)
