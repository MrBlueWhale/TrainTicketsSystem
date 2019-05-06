# 数据库课程设计——火车票售票系统
很烦数据库课程设计？本项目应该能够帮到你~
<br>
TrainTickets为后台工程文件。
train-tickets-front-end为前端工程文件。
<br>

## 系统开发平台：
开发工具：eclipse，webstorm
开发语言：Java，jsp，css，JavaScript
数据库：MySQL
中间件：tomcat 8.0
后台框架：SpringMVC
前端框架：React（前端只是做了一个展示，不是很重要）
<br>

## 系统功能：
在本系统中，前端和后台使用json进行数据交互，下面的每一个功能均对应着一个接口，括号中为接口的URL，具体实现可以参考源代码。

##### 用户层面：
添加用户，即注册。(/register)
根据用户名和密码获取用户的所有信息，即登录。 (/login) 
修改用户。 (/updateUser)

##### 订单层面：
添加订单，在本系统中添加订单就意味着锁定座位。(/lockSeat)
修改订单。(/updateOrder)
删除订单。(/deleteOrder)
根据用户ID获取订单信息。(/queryOrder)

##### 火车层面：
根据车站获取列车ID。(/getTrainByStop)
根据列车ID获取列车信息。(/getTrainByTrainId)
列车换乘查询。(/getTransfer)
查询列车座位剩余。(/getRemainSeats)
查询所有通列车的城市。(/getAllCities)
<br>

## 部署须知：
后台的部署比较简单，将下载的工程打包成war文件后，直接丢到tomcat里，并向localhost:8080/TrainTickets/xxx (xxx为对应的接口)发起post请求就可以了。

前端的部署需要安装node.js
之后进入train-tickets-front-end文件夹，输入npm run start
访问localhost:3000即可。
