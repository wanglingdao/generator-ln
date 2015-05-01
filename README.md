# generator-ln


> Yeoman 生成器，用于生成基于 SeaJS/SPM 的前端项目/组件文件结构。


## 安装

- **安装 yo**

    ```bash
    $ npm install -g yo
    ```

- **安装 generator**

    ```bash
    $ npm install -g generator-ln
    ```

- **安装 spm**

    ```bash
    $ npm install -g spm
    ```

## 使用

### 项目目录结构

- **生成**

    ```bash
    $ yo ln
    ```

- **说明**

    ```
    |-<name> <外部目录，非本脚本生成>
        |-app/ <业务模块>
        |-dist/ <构建后的 APP 文件>
        |-lib/ <通用的第三方库>
            |-seajs/
                |-sea.js
                |-sea-debug.js
            |-config.js <配置文件，READONLY>
            |-config.js.tpl <配置文件模板>
        |-mod/ <通用模块，非业务类>
        |-node_modules/ <NPM 模块>
        |-spm_modules/ <SPM 模块>
        |-theme/ <主题目录>
            |-default/
                |-css/ <样式>
                |-scss/ <SASS>
                |-font/ <字体>
                |-img/ <图片>
        |-.editorconfig
        |-.gitignore
        |-.jshintrc
        |-Gruntfile.js
        |-package.json
        |-README.md
    ```

### 组件目录结构

- **生成**

    ```bash
    $ mkdir <name>
    $ cd <name>
    $ yo ln:module
    ```

- **说明**

    ```
    |-<name> <外部目录，非本脚本生成>
        |-examples/
        |-node_modules/
        |-spm_modules/
        |-tests/
        |-.editorconfig
        |-.gitignore
        |-.jshintrc
        |-.spmignore
        |-.travis.yml
        |-Gruntfile.js
        |-HISTORY.md
        |-index.js
        |-package.json
        |-README.md
    ```
