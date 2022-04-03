### 编程风格
The basic idea is to make sure that every object is designed to have the **smallest possible public interface**, has a lot of internal safety checks  
and is hard to use improperly, and knows how to clean up after itself. We want to **avoid “paired” operations** (e.g. malloc/free, open/close, or new/delete),  
where it might be possible for the second half of the pair not to happen (e.g., if a function returns early or throws an exception).    
Instead, **operations happen in the constructor** to an object, and the **opposite operation happens in the destructor**.   
This style is called “**Resource acquisition is initialization**” or **RAII**.   
  
### 有用的链接
  1. cmake-examples <https://github.com/ttroy50/cmake-examples>
  2. c++ core guilines <http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines>
  3. github handbook  <https://docs.github.com/cn/get-started/using-git/about-git>

### 提醒
 "Send yourself an email "可以使用自己校内smtp服务,或者使用别的邮箱提供的smtp服务.  
 qq邮箱参考 <https://blog.csdn.net/cccccout/article/details/105764940>  注意交互时候使用base64编码
