# Open PDF files in Ionic 6 with File Opener Plugin
# File
[![npm version](https://badge.fury.io/js/%40awesome-cordova-plugins%2Ffile.svg)](https://badge.fury.io/js/%40awesome-cordova-plugins%2Ffile)

## Install
```bash	
npm install cordova-plugin-file --save
npm install @awesome-cordova-plugins/file --save
ionic cap sync
```

```typescript
import { File } from '@awesome-cordova-plugins/file/ngx';

constructor(private file: File) { }

this.file.writeFile(this.file.dataDirectory, 'myFile.pdf', blob, { replace: true }).then((fileEntry) => {
  console.log('File created!', fileEntry);
});
```

# File Opener
[![npm version](https://badge.fury.io/js/%40awesome-cordova-plugins%2Ffile-opener.svg)](https://badge.fury.io/js/%40awesome-cordova-plugins%2Ffile-opener)

## Install
```bash
npm install @awesome-cordova-plugins/file-opener
npm install cordova-plugin-file-opener2 
ionic cap sync
```

```typescript
import { FileOpener } from '@awesome-cordova-plugins/file-opener/ngx';

constructor(private fileOpener: FileOpener) { }


this.fileOpener.open('file:///storage/emulated/0/Download/1.pdf', 'application/pdf')
  .then(() => console.log('File is opened'))
  .catch(e => console.log('Error opening file', e));

```

# Bug Report: 
    
```bash
error: package android.support.v4.content does not exist
```
Install jetifier to fix this issue


# Jetifier
[![npm version](https://badge.fury.io/js/jetifier.svg)](https://badge.fury.io/js/jetifier)

## What is Jetifier?
Jetifier is a tool that helps migrating AndroidX dependencies in your project. It is a part of the AndroidX migration process.

```bash
npm install jetifier --save-dev
npx jetify
```



