2018-5-30  Day03
# 重定向
## 什么是重定向?
- 服务器通知浏览器重新访问一个新的地址.
	  注:
		 服务器可以发送一个302状态码及一个Location消息头(该消息头的值是一个地址,一般称之为重定向地址)给浏览器;浏览器收到之后,会立即向重定向地址发送请求.
![](redirect.png)

- 如何重定向?
	  response.sendRedirect(String url);
	  注:
	    url : 重定向地址.(可以定向到任意可访问的网址)
		      重定向之后,浏览器地址栏的地址会发生变化.

- 细节 : 重定向之前,容器会先清空response对象上存放的所有数据.