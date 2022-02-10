# JD
> jd script

![JD Sync](https://github.com/gclm/jds/actions/workflows/jd-sync.yml/badge.svg)

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
  ql repo https://github.com/gclm/jds.git "jd_|jx_|jddj_" "backUp" "^jd[^_]|USER|JD|function|sendNotify" "main"
  ```
- 国内鸡
  ```
  ql repo https://ghproxy.com/https://github.com/gclm/jds.git "jd_|jx_|jddj_" "backUp" "^jd[^_]|USER|JD|function|sendNotify" "main"
  ```
- crontab
  ```
  40 8-23/4 * * *
  ```

### 参考资料

- [脚本来源](https://github.com/6dylan6/jdpro)
- [使用教程](https://github.com/6dylan6/jdpro)
