# java正则表达式
### 基本步骤

1. **创建Pattern对象**：使用正则表达式编译一个Pattern对象。
2. **创建Matcher对象**：使用Pattern对象的`matcher`方法创建一个Matcher对象。
3. **匹配操作**：使用Matcher对象的各种方法执行匹配操作，例如`find`、`matches`等。

### 示例

#### 示例1：简单匹配

java

复制代码
~~~ java 
import java.util.regex.Pattern;
import java.util.regex.Matcher;

public class RegexExample {
    public static void main(String[] args) {
        // 定义一个正则表达式
        String regex = "foo";
        
        // 创建Pattern对象
        Pattern pattern = Pattern.compile(regex);
        
        // 创建Matcher对象
        Matcher matcher = pattern.matcher("foobarfoo");
        
        // 查找匹配项
        while (matcher.find()) {
            System.out.println("Found match at index " + matcher.start() + " to " + matcher.end());
        }
    }
}
~~~

#### 示例2：使用捕获组

java

复制代码

~~~ java
import java.util.regex.Pattern;
import java.util.regex.Matcher;

public class RegexExample {
    public static void main(String[] args) {
        // 定义一个正则表达式
        String regex = "(\\d{3})-(\\d{2})-(\\d{4})";
        
        // 创建Pattern对象
        Pattern pattern = Pattern.compile(regex);
        
        // 创建Matcher对象
        Matcher matcher = pattern.matcher("123-45-6789");
        
        // 检查整体匹配
        if (matcher.matches()) {
            // 输出每个捕获组的内容
            for (int i = 1; i <= matcher.groupCount(); i++) {
                System.out.println("Group " + i + ": " + matcher.group(i));
            }
        }
    }
}

~~~

#### 示例3：替换文本

java

复制代码

~~~java
import java.util.regex.Pattern;
import java.util.regex.Matcher;

public class RegexExample {
    public static void main(String[] args) {
        // 定义一个正则表达式
        String regex = "\\d";
        
        // 创建Pattern对象
        Pattern pattern = Pattern.compile(regex);
        
        // 创建Matcher对象
        Matcher matcher = pattern.matcher("The year is 2024.");
        
        // 替换所有匹配项
        String result = matcher.replaceAll("#");
        
        System.out.println(result); // 输出：The year is ####.
    }
}

~~~

### 常用正则表达式语法

- **`.`**：匹配任意单个字符
- **`\\d`**：匹配任意数字
- **`\\D`**：匹配任意非数字
- **`\\w`**：匹配任意字母、数字或下划线
- **`\\W`**：匹配任意非字母、非数字、非下划线
- **`\\s`**：匹配任意空白字符
- **`\\S`**：匹配任意非空白字符
- **`*`**：匹配前一个字符零次或多次
- **`+`**：匹配前一个字符一次或多次
- **`?`**：匹配前一个字符零次或一次
- **`{n}`**：匹配前一个字符恰好n次
- **`{n,}`**：匹配前一个字符至少n次
- **`{n,m}`**：匹配前一个字符至少n次，但不超过m次
- **`[]`**：匹配括号内的任意字符
- **`[^]`**：匹配括号内的任意字符，但不包括括号内的字符

匹配




- 不能用正则查找


# 要求分析
例如，“Alan M. Turing”是标准格式，而 “Turing， Alan M.”是相反的格式。
String[] index = {  
    "Dijkstra, E. W.",  
    "Ada Augusta Lovelace",  
    "Alan M. Turing",  
    "von Neumann, John"
    
 标准 "格式（至少在西方国家）是列出
 * 所有名字的顺序（中间名通常缩写为
 * 首字母），然后是姓（家族姓氏）。
 *
 * 反向 "格式是姓在前，逗号在后、
 * 其次是名字（按正常顺序排列；有些名字可缩写为首字母）。
 * 姓名可能缩写为首字母）。这种格式可以
 * 如果索引是按姓氏的字母顺序排列的，那么这种格式可以使在索引中查找特定姓名变得更容易。
 * 按姓氏字母顺序排列。
## to standarfd form

/**  
 * Convert all names in the index that are not already in * standard format to that format. The function does not * return any value, but modifies (entries in) the given index. * @param index The index  
 */


## to reverse form
**
 * 将索引中所有尚未使用
 * 反向格式的名称转换为该格式。该函数不
 * 返回任何值，但会修改给定索引中的条目。
 *
 * 该函数需要识别标准格式的姓名中哪一部分是姓氏。
 * 该函数需要确定标准格式的姓名中哪一部分是姓氏。一般来说，考虑到世界各地不同的
 * 一般来说，考虑到世界上所有不同的姓名约定，这可能会非常复杂。
 * 为了实现这个函数，我们将考虑
 * 以下是简化规则：
 *
 * 出现的姓氏是姓氏的一部分。
 *
 * 出现的姓氏是姓氏的一部分。
 * 小写字母开头的名字也是姓氏的一部分。
 *
 * 例如，在 "约翰-冯-诺依曼 "中，姓氏是 "冯-诺依曼"。
 *
 * @param index 索引
**
     * Convert all names in the index that are not already in reverse format to that format. The function does not return any value, but modifies (entries in) the given index.
     *
     * This function needs to identify what part of a name in standard format is the surname. In general, conidering all the different name conventions around the world, this can be very complex, but
     * for the implementation of this function, we will consider the following simplified rules:
     *
     * -   The last name that appears is part of the surname.
     *
     * -   Any names before the last name that begin with a lowercase letter are also part of the surname.
     * 
     * For example, in "John von Neumann", the surname is "von Neumann".
     *
     * @param index The index



这个算法使用递归来计算组合数，基于组合数的递归性质 C(n,k)=C(n−1,k−1)+C(n−1,k)C(n, k) = C(n-1, k-1) + C(n-1, k)C(n,k)=C(n−1,k−1)+C(n−1,k)。在递归中，处理边界条件时，如果 k=0k = 0k=0 或 k=nk = nk=n，组合数的值为1，这是因为：

1. **k=0k = 0k=0**：从 nnn 个元素中选择 0 个元素的方法只有一种，即什么也不选。因此 C(n,0)=1C(n, 0) = 1C(n,0)=1。
2. **k=nk = nk=n**：从 nnn 个元素中选择所有 nnn 个元素的方法也只有一种，即选择所有元素。因此 C(n,n)=1C(n, n) = 1C(n,n)=1。

这些边界条件确保了递归的基准情况，从而使递归能够终止并返回正确的结果。

这里是该算法的解释：

java

复制代码

`public class Combinations {      // 递归方法计算组合数 C(n, k)     static int choose(int n, int k) {         // 基本情况：如果 k = n 或 k = 0，返回 1         if (k == n || k == 0) {             return 1;         }         // 递归调用，使用组合数的递归性质         return choose(n - 1, k - 1) + choose(n - 1, k);     }      public static void main(String[] args) {         // 测试用例         System.out.println(choose(5, 2));   // 输出 10         System.out.println(choose(6, 2));   // 输出 15         System.out.println(choose(5, 3));   // 输出 10         System.out.println(choose(10, 5));  // 输出 252         System.out.println(choose(20, 10)); // 输出 184756     } }`

### 递归算法的解释：

1. **基准情况**：
    
    - 当 k=0k = 0k=0 时，`choose(n, 0)` 返回 1。
    - 当 k=nk = nk=n 时，`choose(n, n)` 返回 1。
2. **递归步骤**：
    
    - 计算 `choose(n - 1, k - 1)`，这表示从前 n−1n - 1n−1 个元素中选择 k−1k - 1k−1 个元素。
    - 计算 `choose(n - 1, k)`，这表示从前 n−1n - 1n−1 个元素中选择 kkk 个元素。

通过递归调用，算法将问题分解成更小的子问题，直到达到基准情况。基准情况确保递归能够终止，并提供了正确的结果。最终的结果是所有子问题结果的累加。











