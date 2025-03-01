| 字段                    |
| ------------------------- |
| ip                      | 
| addr                    | 
| as.number               | 
| as.name                 | 
| as.info                 | 
| location.latitude       | 
| location.longitude      | 
| country.code            | 
| country.name            | 
| registered_country.code |
| registered_country.name | 
| regions                 | 
| regions_short           | 
| type                    |

### 使用方法

查询其他ipv4：`https://ip.xxx.com/1.1.1.1` `https://ip.xxx.com/?ip=1.1.1.1`

查询其他ipv6：`https://ip.xxx.com/2409:8900:1800::` `https://ip.xxx.com/?ip=2409:8900:1800::`

### Docker 部署


#### 构建镜像

`docker build -t geoip-api .`

#### 运行容器

`docker run -d --name geoip-api -p 5050:8080 geoip-api`

---

### 在线拉取

`docker pull ghcr.io/pseuo/geoip:main`

`docker run --name geoip-api -d -p 5050:8080 ghcr.io/pseuo/geoip`
