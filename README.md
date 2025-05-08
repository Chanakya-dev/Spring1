# Bean.xml
```xml
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
        http://www.springframework.org/schema/beans
        https://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="greetingService" class="com.example.GreetingService"/>

    <bean id="helloService" class="com.example.HelloService">
        <constructor-arg ref="greetingService"/>
    </bean>

</beans>
```
