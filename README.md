##pdf to html （phantom）

将html文件转化为pdf，生成本地文件

##构建方式
```
  npm install phantom --save-dev
```
##API
```javascript
  const instance = await phantom.create();
  const page = await instance.createPage();
  const status = await page.open(path);  //html path
  const content = await page.property('content'); //html content
  await page.render(pdf_path);   //pdf create path
  //this.ctx.body = content;
  await instance.exit();  //exit
```
