# JD
> jd script

## 使用教程

### 青龙面板安装
> 官方仓库：https://github.com/whyour/qinglong
```
docker run -dit \
   -v $PWD/ql/config:/ql/config \
   -v $PWD/ql/log:/ql/log \
   -v $PWD/ql/db:/ql/db \
   -v $PWD/ql/repo:/ql/repo \
   -v $PWD/ql/raw:/ql/raw \
   -v $PWD/ql/scripts:/ql/scripts \
   -v $PWD/ql/jbot:/ql/jbot \
   -p 5700:5700 \
   --name qinglong \
   --hostname qinglong \
   --restart unless-stopped \
   whyour/qinglong:latest
```

### 导入脚本
- 国外鸡
  ```
  ql repo https://github.com/gclm/jd.git "jd_|jx_|getJDCookie" "backUp|icon" "^jd[^_]|USER|sendNotify|sign_graphics_validate|JDJR|JDSign" "main"
  ```
- 国内鸡
  ```
  ql repo https://ghproxy.com/https://github.com/gclm/jd.git "jd_|jx_|getJDCookie" "backUp|icon" "^jd[^_]|USER|sendNotify|sign_graphics_validate|JDJR|JDSign" "main"
  ```
- crontab
  ```
  0 0 0 * * *
  ```

### 环境变量

- [配置参数](https://github.com/gclm/jd/blob/main/githubAction.md)

### 参考资料

- [脚本来源](https://github.com/zero205/JD_tencent_scf/tree/main)
- [使用教程](https://github.com/gclm/jd/blob/main/githubAction.md)
