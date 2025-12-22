**反射 = 在“运行期”获取类的信息，并操作类的结构（属性、方法、构造器）的一种机制**
Java 中，每一个类在 JVM 里，都会有一个对应的 Class 对象
Class<Person> c = Person.class;

这个 Class 对象里，保存了这个类的全部结构信息：
类名、包名 | Class
构造方法     | Constructor
成员变量     | Field
成员方法     | Method
注解            | Annotation
父类、接口 | Class

**反射的一切，起点都是 Class**
获取 Class 对象的 3 种方式
① 类名.class
Class<Person> c = Person.class;

② 对象.getClass()
Person p = new Person();
Class<? extends Person> c = p.getClass();

③ Class.forName()
Class<?> c = Class.forName("com.example.Person");

**invoke 的本质**
JVM 帮你在运行期“找方法 + 调用”

Java 反射是一种让 JVM 在运行期“查看并操作类结构”的机制，是框架的基石，但不适合大量业务代码使用。