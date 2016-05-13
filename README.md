# 想要熟练掌握sourcetree 需要明白的几点
- 什么是工作区、暂存区、本地仓库、远程仓库
- soucetree的工具栏的几个操作的真正含义：<br/>
	丢弃：是本地仓库的内容覆盖到暂存区和工作区<br/>
	暂存：将修改的<br/>


# [测试地址](http://testyunoa.99.com/)

# [wiki地址](http://ued.tming.tmc/wiki/index.php/%E4%BA%91%E5%8A%9E%E5%85%AC%E9%A1%B9%E7%9B%AE%E6%A6%82%E8%BF%B0)


## 项目目录
```
├─ HTML                      # HTML静态页面
│  ├─ org/                   # 组织架构
│  ├─ esop/                  # 审批
│  ├─ home/                  # 首页
│  ├─ login/                 # 登录注册
│  ├─ notice/                # 公告
│  ├─ report/                # 日志
│  └─ registration/          # 签到
│
└─ Theme                     # 风格主题
    ├─ default               # 默认风格
    │  ├─ font/
    │  ├─ images/
    │  ├─ css/
    │  │  ├─ base.css        # 基础CSS
    │  │  └─ extend.css      # 拓展CSS（研发同学专用）
    │  ├─ org/
    │  │  ├─ css/
    │  │  └─ images/
    │  ├─ esop/
    │  ├─ home/
    │  ├─ login/
    │  ├─ notice/
    │  ├─ report/
    │  └─ registration/
    │
    ├─ theme1/               # 风格1
    └─ theme2/               # 风格2
```
- `extend.css`是专门给开发同学调整拓展CSS用的
- 不要让开发的同学直接在其他`.css`上改动调整

***


## 开发目录(src)
```
├─ HTML                     # HTML静态页面
│  ├─ common/               # 通用
│  ├─ org/                  # 组织架构
│  ├─ esop/                 # 审批
│  ├─ home/                 # 首页
│  ├─ login/                # 登录注册
│  ├─ notice/               # 公告
│  ├─ report/               # 日志
│  └─ registration/         # 签到
│
└─ Theme                    # 风格主题
    ├─ default              # 默认风格
    │  ├─ font/             # 图标字体
    │  ├─ images/               
    │  ├─ css/
    │  │  ├─ base.scss      # 基础CSS
    │  │  └─ extend.css     # 拓展CSS（研发同学专用）
    │  │  
    │  ├─ scss/
    │  │  ├─ _reset.scss          # 重置
    │  │  ├─ _setting.scss        # 常用变量&方法
    │  │  ├─ _common.scss         # 通用代码片段
    │  │  ├─ addons/              # 插件
    │  │  ├─ layout/              # 布局
    │  │  └─ ui/                  # 控件   
    │  │  
    │  ├─ org/
    │  │  ├─ css       # 模块CSS入口
    │  │  │  └─ org.scss
    │  │  │  └─ scss/
    │  │  │     ├─ _exam1.scss     
    │  │  │     └─ _exam2.scss    
    │  │  └─ images/
    │  │
    │  ├─ esop/
    │  ├─ home/
    │  ├─ login/
    │  ├─ notice/
    │  ├─ report/
    │  └─ registration/
    │
    ├─ theme1/               # 风格1
    └─ theme2/               # 风格2
```