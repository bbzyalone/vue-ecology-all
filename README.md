# vue-ecology-all


## vite-plugin-commonjs 是一个 Vite 插件，用于将 CommonJS 模块转换为 ES6 模块
```
npm install vite-plugin-commonjs --save-dev
```

** 使用 vite.config.ts**

```
import commonjs from 'vite-plugin-commonjs';

// https://vitejs.dev/config/
export default defineConfig({
  plugins: [
    vue(),
    vueJsx(),
    commonjs(),
  ],
  resolve: {
    alias: {
      '@': fileURLToPath(new URL('./src', import.meta.url))
    }
  }
})
```# vue-ecology-all
