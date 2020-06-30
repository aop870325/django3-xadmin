# 基于原版xadmin修改，兼容python3.8+Django3.0.3
- 直接下载zip包，修改名称为xadmin
- 在 settings.py 文件中的 INSTALLED_APPS，引入
- 安装时缺少包需安装

```
  django
  django-crispy-forms
  django-import-export
  django-reversion
  django-formtools
  future
  httplib2
  six
```
- 配置 urls.py 

```python
import xadmin
...
urlpatterns=[
  path('xadmin/', xadmin.site.urls),  # 后台管理系统页面
]
```

之后参照官方文档配置
