# Blog 만들기
- Vercel 홈페이지 -> Blog Starter Kit -> npx create-next-app --example blog-starter blog-starter-app

## next.config.js

```js
/**
 * @type {import('next').NextConfig}
 */
const nextConfig = {
    output: 'export',
    distDir: 'dist',
    images: {
        unoptimized: true,
    }
}

module.exports = nextConfig
```
- npm run build -> dist 폴더 생성 -> npx serve ./dist
- gitignore 파일에서 -> next.js -> /dist/
- github -> setting -> 

- next.config.js에서 output: 'export' 겹치기 때문에 삭제하고 path: ./dist 로 수정.
name: Static HTML export with Next.js
run: ${{ steps.detect-package-manager.outputs.runner }} next export 

