[https://github.com/yijun-l/jee/blob/main/doc/1-2%20Application%20Server.md](https://github.com/yijun-l/jee/blob/main/doc/1-2%20Application%20Server.md)

## 20261105

Hi Qingbo,

Java EE standards are widely used across Avaya products:
- Wildfly: SMGR, SM
- WebSphere: SM
- Tomcat: AMS, AADS, EP, AES

To better support SMGR, I want to start a Java EE learning session.

Since the topics involve in-depth coding, I want to start with a focused group (As I know, currenlty Jack and Hongjie are qualified), and schedule the session around Jack's availability.

Expected Roadmap: Servlet -  JSP/JSF - Spring Core - EJB - CDI/JNDI/JPA - SpringMVC - Spring Data - Spring Cloud - Cloud-Native App - Vue/React - Spring AI

Topic example: https://github.com/yijun-l/jee/blob/main/doc/1-2%20Application%20Server.md


## 20261110

Hi Team,

Avaya 大量核心产品底层均基于 Java EE 标准构建，并运行在应用服务器上：
- WildFly: SMGR, SM
- WebSphere: SM
- Tomcat: AMS, AADS, AAWG, EP, AES

结合当前的 SMGR T4 工作，打算开一个 J2EE Learning Session，将 Java EE 基础理论与实际的 SMGR PEA 结合起来。

原本想按照我的学习笔记进度来推进，但感觉内容太多了。
 https://github.com/yijun-l/jee/blob/main/doc/1-2%20Application%20Server.md

暂且改为每个 Topic 提前明确讨论重点与前置基础，大家有初步了解后再进行深入探讨。  

第一个topic 就简单聊聊java吧，怎么样？

```java
1. jvm, jre, jdk, java/class file, javac, jps
2. Training like LLM: Legacy coding, IDE coding, vibe coding
3. Programming to an interface
public interface Servlet{
    public void service();
}

public class TestServlet implements Servlet{
    @Override
    public void service(){
        System.out.println("TestServlet is Running!");
    }
}

4. Reflection
Class<?> clazz = forName("TestServlet");
Constructor<?> constructor = clazz.getDeclaredConstructor();

5. IoC (Inversion of Control)
Servlet servlet = constructor.newInstance();
servlet.service();

Code reference: https://github.com/yijun-l/jee/tree/main/mini-server
```
