# 0002_Python_Syntax_Code_Layout_and_Basics / 0008_Identifiers.md

---

# 1. What is an identifier / 什么是标识符

| Type 类型 | Core Idea 核心概念 | How it works 运作方式 | Usage / Example 用途 / 例子 |
|---|---|---|---|
| Identifier 标识符 | An identifier is a name given by the programmer to represent a variable, function, class, or object.<br>标识符是程序员用来表示变量、函数、类或对象的名字。 | Python uses identifiers to refer to data and program components during execution.<br>Python 在执行程序时通过标识符来引用数据和程序结构。 | `age = 20` → `age` is an identifier<br>`def greet():` → `greet` 是标识符 |
| User-defined name 用户自定义名字 | Identifiers are created by the programmer, not by the language itself.<br>标识符是程序员创建的，不是语言预设的。 | You choose meaningful names to represent values or behavior.<br>你通过名字表达数据或行为的含义。 | `total_score`, `student_name`, `calculate_average` |
| Reference label 引用标签 | An identifier acts like a label pointing to a value or object in memory.<br>标识符就像一个标签，指向内存中的值或对象。 | Python does not store values “in variables”, it binds names to objects.<br>Python 实际上是把“名字绑定到对象”。 | `x = 10` → x 指向 10 这个对象 |

---

# 2. Identifier vs Keyword / 标识符 vs 关键字

| Aspect 对比维度 | Identifier 标识符 | Keyword 关键字 |
|---|---|---|
| Ownership 所属 | Programmer 自定义 | Python 语言 |
| Meaning 意义 | Flexible 可自定义 | Fixed 固定 |
| Can rename? 能改吗 | Yes 可以 | No 不可以 |
| Can be variable name? 能当变量名 | Yes | No |
| Example 例子 | `age`, `total`, `name` | `if`, `for`, `def`, `return` |

---

# 3. Rules for identifiers / 标识符命名规则

| Rule 规则 | Explanation 解释 | Valid 正确 | Invalid 错误 |
|---|---|---|---|
| Start rule | Must start with letter or underscore<br>必须字母或下划线开头 | `age`, `_count` | `1age`, `9name` ❌ |
| Characters | Letters, digits, underscore only<br>只能字母数字下划线 | `user1`, `score_2` | `user-name` ❌ |
| No spaces | 不能有空格 | `student_name` | `student name` ❌ |
| No keywords | 不能用关键字 | `value` | `if`, `class` ❌ |
| Case-sensitive | 区分大小写 | `Age`, `age` 不同 | - |
| No symbols | 不允许特殊符号 | `total_price` | `price$`, `@num` ❌ |

---

# 4. Valid vs Invalid identifiers / 正确 vs 错误

| Type | Code | Explanation |
|---|---|---|
| Valid | `age = 20` | 正确命名 |
| Valid | `student_name = "Ali"` | snake_case |
| Invalid | `1age = 20` | 数字开头 ❌ |
| Invalid | `student-name = ""` | 特殊符号 ❌ |
| Invalid | `class = "A"` | keyword ❌ |
| Invalid | `my name = "Ali"` | 空格 ❌ |

---

# 5. Types of identifiers / 标识符类型

| Type 类型 | Definition 定义 | Example 例子 | 中文 |
|---|---|---|---|
| Variable | Stores value | `age = 20` | 变量 |
| Function | Defines behavior | `def greet():` | 函数 |
| Class | Blueprint | `class Student:` | 类 |
| Parameter | Function input | `def add(a, b):` | 参数 |
| Module | File name | `import math` | 模块 |

---

# 6. Naming conventions / 命名规范（PEP8）

| Type 类型 | Style 规则 | Example 例子 | 中文 |
|---|---|---|---|
| Variable | snake_case | `total_score` | 小写+下划线 |
| Function | snake_case | `calculate_sum()` | 函数命名 |
| Class | PascalCase | `StudentRecord` | 类名 |
| Constant | UPPER_CASE | `MAX_SIZE` | 常量 |
| Private | _leading underscore | `_hidden` | 内部使用 |

---

# 7. Good vs Bad naming / 好 vs 坏命名

| Type 类型 | Bad ❌ | Good ✅ | Reason 原因 |
|---|---|---|---|
| Variable | `x` | `age` | 可读性 |
| Variable | `a1` | `student_count` | 清晰 |
| Function | `f()` | `calculate_total()` | 表达行为 |
| List | `l` | `scores_list` | 避免混淆 |

---

# 8. Meaningful naming principles / 命名原则

| Principle 原则 | Explanation 解释 | Example |
|---|---|---|
| Descriptive | 表达用途 | `total_price` |
| Avoid vague | 避免模糊 | ❌ `data` → ✅ `user_data` |
| Readable | 易读优先 | `student_age` |
| Not too long | 不要过长 | ❌ 超长变量名 |

---

# 9. Identifier behavior / 标识符本质

| Concept 概念 | Explanation 解释 | Example |
|---|---|---|
| Name binding | 名字绑定对象 | `x = 10` |
| Reference | 指向对象 | `a = b` |
| Not container | 不是盒子 | Python 是引用模型 |

---

# 10. Example / 示例

| Code | Explanation |
|---|---|
| `a = 10` | a 指向 10 |
| `b = a` | b 指向同一个对象 |

---

# 11. Common mistakes / 常见错误

| Mistake 错误 | Result 结果 | Why |
|---|---|---|
| Keyword as name | Syntax error | 被占用 |
| Start with number | Error | 规则不允许 |
| Using symbols | Error | 不合法 |
| Case confusion | Bug | 区分大小写 |
| Bad naming | Hard to read | 可读性差 |

---

# 12. Practical example / 实战对比

| Bad Code ❌ | Good Code ✅ |
|---|---|
| `x = 10`<br>`y = 20`<br>`z = x + y` | `first_number = 10`<br>`second_number = 20`<br>`total_sum = first_number + second_number` |

---

# 13. Memory thinking / 内存理解

| Concept | Explanation |
|---|---|
| Identifier | 名字 |
| Object | 数据 |
| Binding | 名字指向数据 |

---

# 14. Advanced preview / 进阶预告

| Topic | Explanation |
|---|---|
| Scope | 作用域 |
| Shadowing | 覆盖变量 |
| Lifetime | 生命周期 |

---

# 15. Self-check / 自我检查

| Question |
|---|
| 我能解释 identifier 吗？ |
| 我知道命名规则吗？ |
| 我能写合法变量名吗？ |
| 我能写清晰名字吗？ |

---

# Key Takeaways / 核心总结

| Point | Explanation |
|---|---|
| Identifier = 名字 | 程序员定义 |
| Keyword ≠ Identifier | 不能用 |
| Naming rules | 必须遵守 |
| Good naming | 很重要 |
| Case-sensitive | 要注意 |

---
