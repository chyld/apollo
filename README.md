![Apollo](https://raw.githubusercontent.com/chyld/apollo/master/client/assets/screenshot.png)

## Frontend Gulp Template + AWS S3 Upload

### Description
This front end template allows you to get your browser-based code up and running quickly. An example:

```
git clone https://github.com/chyld/front-end-prototype my-app
cd my-app
./setup.sh
gulp
```

The base project is now setup and your browser should have automatically opened ```http://localhost:3000```. Open the project files in your editor of choice. Edit/Add files in the ```client``` directory. As you edit/add files, gulp will translate/concat/morph files from the ```client``` directory to the ```public``` directory. The browser will automatically refresh with your new changes. Once you're ready to push/deploy the code to your Amazon S3 bucket:

```
export AWS_SECRET_ACCESS_KEY=your-secret-key
export AWS_ACCESS_KEY_ID=your-access-key
export AWS_BUCKET=your-bucket-name
export AWS_REGION=your-region
NODE_ENV=production gulp aws:publish:full
```

Your web application is now live!

### Languages
- Jade
- Less
- JS

### 3rd Party Libraries
- Lodash
- Font Awesome

### Build Tools
- Gulp
- Bower
- AWS S3 Bucket Upload
- Jade/Less Transpiler
- JsHint
- Clean
- Copy
- Size
- Watch
- Concat
- Uglify/Minify
- Rename
- Browser Sync w/Live Reload
