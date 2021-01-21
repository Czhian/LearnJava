# Lombok的使用

## 1.概述

Lombok是一个Java工具类，通过自定义注解，可以消除日常开发过程中的冗余代码，达到精简代码的目的

## 2.Lombok常用注解

@Getter：用在类的属性上，为属性自动生成getter方法

@Setter：用在类的属性上，为属性自动生成setter方法

@ToString：用在类上，为类自动生成toString()方法

@EqualsAndHashCode：用在类上，为类生成equals()和hashCode()方法

@AllArgsConstructor：

用在类上，可以自动引入Bean，不用再写@Autowired，注入多个Bean的时候更加清晰

**@RequiredArgsConstructor**：只会构造注入final修饰的属性，推荐使用

@NoArgsConstructor：自动生成无参构造

**@Data**：添加在类上，可以自动为类生成getter,setter方法，equals，hashCode方法，toString方法

@Value：用在类上面，与@Data类似，不同的是@Value会把类的属性转换成final修饰的，所以不会有setter方法，注意Lombok的@Value和Spring的@Value是不同的，

**@Slf4j**：自动添加日志框架，在类上使用

@NonNull：用在类的属性上，如果类的属性为null则抛出异常

@Cleanup：用在局部变量上，作用域结束时自动释放资源

**@Builder**：用在类上，表示自动为类添加Builder模式，可以通过builder来构建对象，使用这个以后就不需要再声明构造函数了

@Synchronized：用在方法上，自动添加同步锁

**@SneakyThrows**：用在类的方法上面，自动为类添加try catch模块，不需要再编写异常捕获代码

