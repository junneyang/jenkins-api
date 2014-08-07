jenkins-api
==========

usage of jenkins api,mainly for json api.

【jenkins】
1、查询jenkins任务列表详情
curl -X POST http://cq01-rdqa-pool094.cq01.baidu.com:8080/api/json?pretty=true
2、查询jenkins某一job详情
curl -X POST http://cq01-rdqa-pool094.cq01.baidu.com:8080/job/jenkinsAPI/api/json?pretty=true
3、带参数启动某一job
curl -X POST http://cq01-rdqa-pool094.cq01.baidu.com:8080/job/jenkinsAPI/buildWithParameters?time=10
4、查询jenkins任务队列列表
curl -X POST http://cq01-rdqa-pool094.cq01.baidu.com:8080/queue/api/json?pretty=true
5、查询某一job实时测试状态
http://cq01-rdqa-pool094.cq01.baidu.com:8080/job/jenkinsAPI/10/api/json?pretty=true
http://cq01-rdqa-pool094.cq01.baidu.com:8080/job/jenkinsAPI/10/api/json?tree=building
6、查询某一job控制台输出
http://cq01-rdqa-pool094.cq01.baidu.com:8080/job/jenkinsAPI/10/logText/progressiveText?start=0

