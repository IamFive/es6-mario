# 🎮 ES6-Mario

这是一个用HTML5和原生ES6等新特性及语法写成的`Web 游戏`。

主体结构学习自 [[Meth Meth Method On Youtube](https://www.youtube.com/channel/UC8A0M0eDttdB11MHxX58vXQ)](https://www.youtube.com/watch?v=g-FpDQ8Eqw8&index=1&list=PLS8HfBXv9ZWWe8zXrViYbIM2Hhylx8DZx) by [@Meth Meth Method][https://github.com/meth-meth-method] .

非常感谢 [@Meth Meth Method][https://github.com/meth-meth-method] 及其作者  [@pomler][https://github.com/pomle]。



## 运行

```
git clone https://github.com/JuniorTour/es6-mario

cd es6-mario

npm install

npm run dev     // 在 http://localhost:8080 启动开发服务器

npm run build   // 打包编译源代码至 ./public/dist

npm run prod    // 打包编译源代码至 ./public/dist 并且 在 http://localhost:666 启动生产环境服务器

```



## Demo

### 在线 Demo

# [Play es6-mario Online]()

![QR-CODE-es6-mario]()


### Gif Demo

![mario-eg-1-60fps.gif](./public/notes/mario-eg-1-60fps.gif)

![mario-eg-2-60fps.gif](./public/notes/mario-eg-2-60fps.gif)



## 经验总结

0. 经常整理代码

可以通过`借助module语法分离声明和实现`，`构建类`等来实现。
([More.........](https://github.com/JuniorTour/es6-mario/blob/master/public/notes/notes.md))



## 关键点总结记录

0. Es6 语法

- <1> Module

``` javascript

<script type="module" src="/js/main.js"></script>

import {loadLevel} from './loader.js'
import {loadBackgroundSprites, loadMarioSprite} from './sprites.js'

```

- <2> Super Class - 超类
  ([More.........](https://github.com/JuniorTour/es6-mario/blob/master/public/notes/notes.md))





## ToDo-List

| No.  | Content                                    | Finish Date | Extra                                                                                                          |
| ---- | -------------------------- | ----------- | ----------------------------------------                                        |
| 0    | 基础结构                                     | 2018/2/14   | 春节前日                                                                                                  |
| 1    | 打包工具                                     | 2018/3/1      | 为了实现更好的兼容性和性能。                                                           |
| 2    | 移动端兼容                                | 2018/3/4      | 为了支持目前互联网的主流。                                                               |
| 3    | 原版地图和游戏内容                  | 2018/3/1      |                                                                                                                |
| 4    | 性能优化                                    |                         | 尝试让低端设备（iPhone se,...）也能以较为流畅的帧数运行               |



## 文件结构

```javascript
|__ public                          主文件夹
  |__ index.html
  |__ assets
      |__ img
        |__ characters.gif
        |__ font.png
        |__ tiles.png
      |__ levels                    关卡内容配置
        |__ 1-1.json
      |__ sound
        |__ overworld-bgm.mp3
      |__ sprites                   角色精灵（雪碧图）配置
        |__ goomba.json
        |__ koopa.json
        |__ mario.json
        |__ overworld.json
        |__ underworld.json
  |__ build
    |__ prod-server.js          生产环境服务器
    |__ webpack.config.js     webpack配置文件
  |__ css
    |__ ......
  |__ js
    |__ entities
      |__ Goomba.js
      |__ Koopa.js
      |__ Mario.js
    |__ input                       键盘及触控操作输入控制
      |__ ......
    |__ layers
      |__ background.js
      |__ camera.js
      |__ collision.js
      |__ dashboard.js
      |__ sprites.js
    |__ loaders
      |__ font.js
      |__ level.js
    |__ polyfill                    兼容性垫片
      |__ ......
    |__ traits                      游戏内角色特性
      |__ Go.js
      |__ Jump.js
      |__ Killable.js
      |__ PendulumMove.js
      |__ Physics.js
      |__ PlayerController.js
      |__ Solid.js
      |__ Stomer.js
      |__ Velocity.js
    |__ anim.js
    |__ BoundingBox.js
    |__ Camera.js
    |__ compositor.js
    |__ debug.js
    |__ entities.js
    |__ Entity.js
    |__ EntityCollider.js
    |__ input.js
    |__ KeyboardState.js
    |__ main.js
    |__ math.js
    |__ sprites.js
    |__ SpriteSheet.js
    |__ TileCollider.js
    |__ TileResolver.js
    |__ Timer.js
    |__ Level.js
    |__ loader.js
  |__ notes
    |__ ......
|__ .gitignore
|__ package.json
|__ README.md

```


## 结语

非常渴望听到你的意见！欢迎通过各种方式联系我：

My GitHub: [@JuniorTour](https://github.com/JuniorTour).

My Email: [juniortour@qq.com](mailto:juniortour@qq.com).