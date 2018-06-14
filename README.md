## html to pdf/png （phantom）

将html文件转化为pdf，生成本地文件

### 构建方式
```
  npm install phantom --save-dev
```
### API
```javascript
  const instance = await phantom.create();
  const page = await instance.createPage();
  const status = await page.open(path);  //html path
  const content = await page.property('content'); //html content
  await page.render(pdf_path);   //pdf create path
  //this.ctx.body = content;
  await instance.exit();  //exit
```

=====================================================================================

## pdf to html （pdftohtmljs  +  pdf2htmlEX）

将pdf文件转化为html，生成本地文件

### 构建方式
```
  npm install pdftohtmljs --save-dev
  blew install pdf2htmlEX   (macOS)
```
### API
```javascript
  const converter = new pdftohtml(pdf-path, html-path);
  converter.convert('ipad').then(function() {
    console.log("Success");
  }).catch(function(err) {
    console.error("Conversion error: " + err);
  });
  converter.progress(function(ret) {
    console.log((ret.current*100.0)/ret.total + " %");
  });
```

