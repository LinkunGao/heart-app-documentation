The documentation hosted on readthedocs.

see:
https://heart-app-documentation.readthedocs.io/

## 关于在 readthedocs 中 override theme css 样式的步骤

- 在 \_static 下创建 css 文件夹， 将 css 文件存放在此处， 例如 override.css
  ```bash
      在其内部控制更改或新增theme的样式
      .highlight {
              background: rgba(220, 220, 220, 0.7) !important;
          }
        // .highlight 可以通过在Google browser 中查看需要控制模块的类名，然后对其进行控制
  ```
- 在 conf.py 中，进行如下配置：
  ```
      html_css_files = [
                  'css/theme_overrides.css',
              ]
  ```

see: https://docs.readthedocs.io/en/stable/guides/adding-custom-css.html
