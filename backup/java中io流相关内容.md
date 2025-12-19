**一、字节流（Byte Stream）**

**（1）文件字节流（读取 / 写入图片、音频、视频，文件拷贝（通用方案），处理未知格式文件）**

FileInputStream | 输入 | 从文件读字节

FileOutputStream | 输出 | 向文件写字节

**（2）缓冲字节流**（大文件 I/O，网络数据流，文件拷贝性能优化）

BufferedInputStream | 输入 | 提高字节读取效率

BufferedOutputStream | 输出 | 提高字节写入效率

**（3）内存字节流（中间缓存，二进制协议拼装，单元测试）**

ByteArrayInputStream | 输入 | 从 byte[] 读

ByteArrayOutputStream | 输出 | 写到 byte[]

**（4）对象流（基于字节）**

ObjectInputStream | 输入 | 反序列化对象

ObjectOutputStream | 输出 | 序列化对象


**二、字符流（Character Stream）**

**（1）文件字符流(简单文本处理,简单文本处理)**

FileReader | 输入 | 从文件读字符

FileWriter | 输出 | 向文件写字符

**（2）缓冲字符流(按行处理文本,配置文件读取,日志解析)**

BufferedReader | 输入 | 高效读字符 / 行

BufferedWriter | 输出 | 高效写字符

**（3）转换流（编码边界）明确指定编码（UTF-8 / GBK）,网络 / 文件文本读取**

InputStreamReader | 输入 | 字节 → 字符

OutputStreamWriter | 输出 | 字符 → 字节

**（4）内存字符流(模板渲染,文本拼接,测试)**

StringReader | 输入 | 从 String 读

StringWriter | 输出 | 写到 String

