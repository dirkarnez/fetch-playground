fetch-playground
================
### Notes
- There is no specific returns / indicator for CORS error in `fetch` API

### Features
- [x] `AbortController`
  - [AbortController - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/AbortController)
- [ ] Cache / No Cache

### Tutorials
- https://github.com/octokit/request.js/blob/main/src/fetch-wrapper.ts

### Download (client-side)
```
.then(d => d.blob())
.then(blob => {
      const downloadUrl = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = downloadUrl;
      a.download = `${new Date().getTime()}`;
      document.body.appendChild(a);
      a.click();
      URL.revokeObjectURL(downloadUrl);
      setTimeout(resolve, 100);
})
```
