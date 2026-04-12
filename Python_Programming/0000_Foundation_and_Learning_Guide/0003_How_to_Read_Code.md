# 1\. What "reading code" really means / 什么叫"读代码"

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Code Reading**<br><br>**读代码** | Reading code does not mean reading it like a storybook. It means understanding what the program is trying to do, how it is organized, and how data moves through it.<br><br>读代码不是像读故事书那样读，而是理解程序想做什么、如何组织、以及数据怎样流动。 | When you read code properly, you identify purpose, inputs, processing steps, conditions, loops, functions, outputs, and relationships between parts.<br><br>当你正确读代码时，你会识别：目的、输入、处理步骤、条件、循环、函数、输出，以及各部分之间的关系。 | Example: In a student score program, you do not only see `total += score`; you understand that the program is accumulating marks to calculate a final result.<br><br>例子：在学生成绩程序里，你不只是看到 `total += score`，而是知道程序在累加分数，为了最后计算结果。 |
| **Understanding Structure**<br><br>**理解结构** | Good code reading starts with structure, not with tiny details first.<br><br>好的读代码方式，先看结构，不是先陷进细节。 | You first ask: What is this program for? What are its major parts? Then you zoom into smaller lines and behaviors.<br><br>你会先问：这个程序做什么？主要部分有哪些？然后再放大看每一行细节和行为。 | Example: Before reading all lines in a menu program, first see where the menu is printed, where user input is taken, and where each option is handled.<br><br>例子：看菜单程序时，不要先逐字逐行看，而是先找菜单在哪里显示、输入在哪里接收、选项在哪里处理。 |
| **Reading for Meaning**<br><br>**为意义而读** | Code should be read for meaning, not only syntax recognition.<br><br>读代码时要读“意义”，不只是认出语法。 | A line may be syntactically simple but logically important. You must ask what role it plays in the whole program.<br><br>某一行语法上可能很简单，但逻辑上很重要；你必须问它在整个程序中扮演什么角色。 | Example: `if password == saved_password:` is not just a comparison line; it is the security gate of the login logic.<br><br>例子：`if password == saved_password:` 不只是比较语句，它是登录逻辑的安全门。 |
| **Reading as Thinking**<br><br>**读代码也是思考** | Reading code is an active thinking process, not passive viewing.<br><br>读代码是主动思考，不是被动观看。 | You should constantly predict, trace, question, and connect code parts while reading.<br><br>你在读代码时，应该不断预测、追踪、提问、连接代码部分。 | Example: Before running code, you should ask: What values will this variable have? How many times will this loop run? Which branch will execute?<br><br>例子：运行代码前，你应该先问：这个变量会是什么值？循环会跑几次？会进入哪个分支？ |

# 2\. Why reading code is a core programming skill / 为什么读代码是核心能力

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Foundation Skill**<br><br>**基础核心技能** | You will read far more code than you write during learning and real development.<br><br>无论在学习还是实际开发中，你读的代码通常会比你自己写的更多。 | Learning examples, tutorials, documentation snippets, teammate code, old projects, and bug traces all require reading skill.<br><br>学习例子、教程、文档片段、队友代码、旧项目和报错线索，全都需要读代码能力。 | Example: To fix a bug, you often first read existing code before changing anything.<br><br>例子：修 bug 时，通常先要读已有代码，再决定改什么。 |
| **Bridge to Writing**<br><br>**连接“看懂”和“会写”** | Good writing usually grows from good reading.<br><br>会写代码，通常建立在会读代码之上。 | When you read enough patterns, your brain starts recognizing reusable structures and solution shapes.<br><br>当你读过足够多模式后，大脑会开始识别可重复使用的结构和解法形状。 | Example: Reading many function examples helps you later design your own functions naturally.<br><br>例子：看多了函数例子后，你后来自己设计函数会更自然。 |
| **Essential for Debugging**<br><br>**调试必备能力** | Debugging is impossible without reading code carefully.<br><br>不会仔细读代码，就无法真正调试。 | Bugs are found by tracing what the code actually does, not by guessing emotionally.<br><br>bug 是通过追踪代码实际在做什么找到的，不是靠情绪猜测。 | Example: A wrong output often comes from a line you misread or a branch you assumed incorrectly.<br><br>例子：输出错误常常来自你看错某一行，或者误判了某个分支。 |
| **Essential for Growth**<br><br>**成长必备能力** | The more advanced the topic becomes, the more code reading matters.<br><br>越到后面进阶内容，读代码就越重要。 | Advanced Python topics like libraries, APIs, classes, decorators, and frameworks often require understanding code that you did not write yourself.<br><br>像库、API、类、装饰器、框架这些进阶内容，通常都需要理解不是你自己写的代码。 | Example: When learning Pandas or Flask, you constantly read examples before building your own solution.<br><br>例子：学习 Pandas 或 Flask 时，你会不断先看例子，再自己搭出解决方案。 |

# 3\. The biggest mistake when reading code / 读代码时最大的错误

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Reading word by word**<br><br>**逐字逐行机械读** | Many beginners read code like plain text, without seeing structure or purpose.<br><br>很多初学者像读普通文字那样读代码，却没有看到结构和目的。 | This causes mental overload because every line feels equally important, even though some lines are structural and some are only supporting details.<br><br>这样会让大脑过载，因为每一行看起来都一样重要，但其实有些行是骨架，有些只是细节。 | Example: In a function, the function definition and return line may matter more first than every `print` inside it.<br><br>例子：在函数里，一开始通常更应该先看函数定义和 `return`，而不是先陷进里面每个 `print`。 |
| **Ignoring purpose**<br><br>**忽略目的** | If you do not know what the program is trying to achieve, every line feels random.<br><br>如果你不知道程序想达成什么目标，每一行都会看起来很随机。 | Purpose acts like a map. Without it, you cannot judge whether a line is storing data, transforming data, checking conditions, or producing output.<br><br>目的就像地图；没有它，你就难以判断某一行是在存数据、改数据、做判断还是输出结果。 | Example: A sorting program makes much more sense once you know the goal is “to arrange values from smallest to largest.”<br><br>例子：一个排序程序，只有在你先知道目标是“把值从小到大排列”后，才会变得容易理解。 |
| **Trying to understand everything instantly**<br><br>**想一次全部看懂** | Beginners often expect immediate full understanding, which is unrealistic for unfamiliar code.<br><br>初学者常常期待第一次就完全看懂，这对陌生代码来说并不现实。 | Real understanding often comes in layers: first purpose, then structure, then data flow, then details, then edge cases.<br><br>真正的理解通常是分层来的：先目的、再结构、再数据流、再细节、再边界情况。 | Example: A long file may only become clear after reading it two or three times with different focus each time.<br><br>例子：一个长文件，往往要看两三遍，而且每一遍的关注点都不同，才会真正清楚。 |
| **Not tracing values**<br><br>**不追踪变量值** | Code cannot be understood well if you ignore how variables change over time.<br><br>如果你忽略变量如何随时间改变，就很难真正看懂代码。 | Variables carry the state of the program. Reading code requires tracking their changes through assignments, conditions, loops, and function calls.<br><br>变量承载程序状态；要看懂代码，就必须追踪它们在赋值、判断、循环和函数调用中的变化。 | Example: `count += 1` only becomes meaningful when you notice how often it runs and what started in `count` before the loop.<br><br>例子：`count += 1` 只有在你知道它执行几次、以及 `count` 一开始是什么值时，才真正有意义。 |

# 4\. The correct order for reading code / 正确的读代码顺序

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Start with the goal**<br><br>**先看目标** | The first question should be: What is this code trying to do?<br><br>第一件事应该问：这段代码到底想做什么？ | Once the goal is clear, each code block becomes easier to interpret in context.<br><br>一旦目标清楚，各个代码块就更容易放回上下文中理解。 | Example: “This program calculates average marks” gives meaning to input, summing, counting, and division lines.<br><br>例子：“这个程序是在计算平均分”会让输入、求和、计数、除法这些行立刻有意义。 |
| **Then identify structure**<br><br>**再找结构** | After knowing the goal, identify the major parts of the program.<br><br>知道目标后，再识别程序的主要结构。 | Look for blocks such as setup, input, processing, conditional logic, loops, function definitions, and output.<br><br>去找像初始化、输入、处理、条件逻辑、循环、函数定义和输出这些区块。 | Example: A menu program often has a menu display block, an input block, and separate option-handling blocks.<br><br>例子：菜单程序通常会有菜单显示区、输入区、以及分别处理各选项的区块。 |
| **Then trace data flow**<br><br>**再追踪数据流** | Once structure is clear, ask how data enters, changes, and leaves the program.<br><br>结构清楚后，再问数据怎样进入、怎样改变、怎样离开程序。 | Follow variables and returned values through the code path.<br><br>跟着变量和返回值去追踪代码路径。 | Example: User enters a number → number stored in variable → loop uses it → result printed.<br><br>例子：用户输入数字 → 数字存进变量 → 循环使用它 → 最后输出结果。 |
| **Finally inspect details**<br><br>**最后再看细节** | Only after goal, structure, and data flow are clear should you focus deeply on detailed syntax or specific lines.<br><br>只有在目标、结构和数据流都清楚后，才应该深入看具体语法和某几行细节。 | This prevents getting lost in unimportant detail too early.<br><br>这样可以避免太早在细节里迷路。 | Example: First understand that a function validates input; then inspect the exact condition checks inside it.<br><br>例子：先知道某个函数是在做输入验证，再深入看它内部具体条件。 |

# 5\. How to identify the purpose of a code block / 怎样判断一个代码块的目的

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Purpose Detection**<br><br>**判断目的** | Every code block has a role inside the larger program.<br><br>每个代码块在大程序里都有自己的角色。 | You can identify the role by asking what effect the block has on program behavior or data.<br><br>你可以通过问“这个区块对程序行为或数据造成了什么影响”来判断它的角色。 | Example: A block may collect input, update totals, search for an item, or display results.<br><br>例子：一个区块可能是在收集输入、更新总数、查找项目，或者显示结果。 |
| **Input Block**<br><br>**输入区块** | An input block gets data from the user, a file, or another source.<br><br>输入区块会从用户、文件或其他来源取得数据。 | It usually contains `input()`, file reading, API responses, or variable setup from external data.<br><br>它通常包含 `input()`、文件读取、API 回应，或来自外部数据的变量设置。 | Example: `name = input("Enter your name: ")` is an input block line.<br><br>例子：`name = input("Enter your name: ")` 就是输入区块的一行。 |
| **Processing Block**<br><br>**处理区块** | A processing block transforms or computes data.<br><br>处理区块会转换或计算数据。 | It may use arithmetic, loops, method calls, or function calls to change existing values into useful results.<br><br>它可能会用运算、循环、方法调用或函数调用，把原始值变成有用结果。 | Example: `average = total / count` is a processing line.<br><br>例子：`average = total / count` 是处理行。 |
| **Decision Block**<br><br>**判断区块** | A decision block chooses one path over another.<br><br>判断区块会决定走哪一条路径。 | It usually contains `if`, `elif`, `else`, or other branching logic.<br><br>它通常包含 `if`、`elif`、`else` 或其他分支逻辑。 | Example: `if age >= 18:` decides whether the user is treated as adult or not.<br><br>例子：`if age >= 18:` 决定用户是否被当成成年人。 |
| **Loop Block**<br><br>**循环区块** | A loop block repeats work.<br><br>循环区块负责重复工作。 | It executes a body multiple times based on items, range, or a condition.<br><br>它会根据项目、范围或条件多次执行一段代码。 | Example: `for score in scores:` repeats the same action for every score.<br><br>例子：`for score in scores:` 会对每个分数重复相同行为。 |
| **Output Block**<br><br>**输出区块** | An output block shows or returns the final result.<br><br>输出区块会显示或返回最终结果。 | It often uses `print()` or `return` to expose the program's result to the user or to another function.<br><br>它通常使用 `print()` 或 `return` 把结果给用户或交给其他函数。 | Example: `print("Average:", average)` is an output line.<br><br>例子：`print("Average:", average)` 是输出行。 |

# 6\. How to read Python code by structure / 怎样按 Python 结构读代码

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Indentation matters**<br><br>**缩进决定结构** | In Python, indentation is not decoration. It defines code blocks.<br><br>在 Python 里，缩进不是装饰，而是区块结构本身。 | Lines aligned at the same indentation level often belong to the same structural block; indented lines belong inside a parent structure.<br><br>同一层缩进的行通常属于同一个结构区块；被缩进的行则属于上层结构内部。 | Example: All lines under an `if` that are indented belong to the `if` block.<br><br>例子：`if` 下面所有有缩进的行，都属于那个 `if` 区块。 |
| **Read blocks, not isolated lines**<br><br>**读区块，不只读单行** | Python code should usually be read block by block, not as disconnected single lines.<br><br>读 Python 代码时，通常要按区块读，而不是把每一行当成互不相关的单行。 | A loop block, condition block, and function block each have their own internal meaning and role.<br><br>循环区块、条件区块、函数区块各自都有整体意义和角色。 | Example: When seeing a `for` loop, read the loop header and the entire indented body together.<br><br>例子：看到 `for` 循环时，要把循环头和整段缩进主体一起读。 |
| **Headers introduce meaning**<br><br>**结构头决定含义** | Certain lines introduce whole structures, such as `if`, `for`, `while`, `def`, and `class`.<br><br>有些行会引入整个结构，例如 `if`、`for`、`while`、`def` 和 `class`。 | These header lines tell you what kind of block follows and how to interpret it.<br><br>这些结构头会告诉你，后面跟的是哪种区块，以及应该怎样理解它。 | Example: `def calculate_total(prices):` tells you that the next block defines reusable behavior with input called `prices`.<br><br>例子：`def calculate_total(prices):` 表示接下来这个区块在定义一个可重复使用的行为，输入叫 `prices`。 |
| **Return closes the purpose of a function**<br><br>**return 会收束函数目的** | In functions, `return` often reveals what result the function is meant to produce.<br><br>在函数里，`return` 往往最能说明这个函数到底想产出什么。 | Reading the return value helps you understand the function's purpose even before every detail is clear.<br><br>先看返回值，可以帮助你在还没完全懂细节前，先把握函数目的。 | Example: `return total / count` strongly suggests the function is producing an average.<br><br>例子：`return total / count` 很明显暗示这个函数是在产出平均值。 |

# 7\. How to trace variables while reading / 读代码时怎样追踪变量

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Variable Tracing**<br><br>**变量追踪** | To understand code, you must watch how variable values change over time.<br><br>要看懂代码，就必须看变量的值怎样随时间变化。 | Start from the first assignment, then update your mental model every time the variable is changed, compared, passed, or returned.<br><br>从第一次赋值开始，每当变量被修改、比较、传入函数或返回时，都要更新你的脑内模型。 | Example: If `total = 0` and later `total += score`, then `total` is accumulating values rather than storing just one final score.<br><br>例子：如果 `total = 0`，后面又有 `total += score`，那 `total` 是在累加，而不是只存一个分数。 |
| **Track initial value**<br><br>**先看初始值** | A variable's starting value often explains its role.<br><br>变量的初始值通常能说明它的角色。 | Counters often start at `0`, flags often start as `False`, and collections may start as empty list or dict.<br><br>计数器常从 `0` 开始，标记常从 `False` 开始，集合可能从空列表或空字典开始。 | Example: `count = 0` suggests counting behavior; `found = False` suggests a search flag.<br><br>例子：`count = 0` 通常表示计数；`found = False` 通常表示查找标记。 |
| **Track every update**<br><br>**追踪每次更新** | A variable may change multiple times, and every change matters.<br><br>变量可能会改变很多次，而每次改变都很重要。 | Updates can happen through assignment, arithmetic, method calls, input replacement, or function returns.<br><br>变量可以通过赋值、运算、方法调用、输入覆盖或函数返回值来更新。 | Example: `name = input(...)` replaces any previous value of `name` with new user input.<br><br>例子：`name = input(...)` 会用用户的新输入，替换 `name` 之前的值。 |
| **Observe when used in conditions**<br><br>**注意它何时参与判断** | A variable's meaning is often revealed when it is used in a condition.<br><br>变量在条件里出现时，往往最能暴露它的意义。 | Conditions show what threshold, state, or category the variable is controlling.<br><br>条件会显示这个变量在控制什么阈值、状态或类别。 | Example: `if count == 0:` means `count` is being used to detect emptiness or no results.<br><br>例子：`if count == 0:` 表示 `count` 被用来判断“是否为空”或“是否没有结果”。 |

# 8\. How to read conditions / 怎样读条件判断

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Condition Reading**<br><br>**读条件** | A condition should be read as a question the program is asking.<br><br>读条件时，要把它当成程序在问的一个问题。 | The program evaluates whether the condition is true or false, then chooses a path accordingly.<br><br>程序会判断条件是真是假，然后根据结果选择路径。 | Example: `if age >= 18:` should be read as “Is age at least 18?”<br><br>例子：`if age >= 18:` 应该读成“age 是否至少 18？” |
| **Branch meaning**<br><br>**分支含义** | Each branch represents a different behavior path.<br><br>每个分支都代表不同的行为路径。 | The `if` block is executed when the condition is true; the `else` block handles the opposite case.<br><br>`if` 区块在条件为真时执行；`else` 区块处理相反情况。 | Example: In login logic, one branch grants access and another denies it.<br><br>例子：在登录逻辑里，一个分支允许进入，另一个分支拒绝进入。 |
| **Read logical operators carefully**<br><br>**仔细读逻辑运算符** | `and`, `or`, and `not` change the exact meaning of the condition.<br><br>`and`、`or`、`not` 会改变条件的确切含义。 | These operators combine or invert smaller conditions, so reading them loosely can cause misunderstanding.<br><br>它们会组合或反转较小条件；如果读得太随便，就会误解逻辑。 | Example: `age >= 18 and has_id` means both conditions must be true, not just one.<br><br>例子：`age >= 18 and has_id` 表示两个条件都要成立，不是只要一个。 |
| **Condition role**<br><br>**条件的角色** | Conditions are often used for validation, classification, permissions, searching, or loop control.<br><br>条件常用于验证、分类、权限判断、搜索或控制循环。 | Knowing the role helps you understand why the condition exists at that point in the program.<br><br>知道条件的角色，可以帮助你理解为什么它会出现在程序的那个位置。 | Example: `if not items:` may exist to handle an empty collection before processing begins.<br><br>例子：`if not items:` 可能是为了在处理开始前，先处理“集合为空”的情况。 |

# 9\. How to read loops / 怎样读循环

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Loop Reading**<br><br>**读循环** | A loop should be read as repeated work, not as many separate copies of code.<br><br>读循环时，要把它看成“重复工作”，而不是很多段不同代码。 | The loop header tells you what controls the repetition; the loop body tells you what action is repeated.<br><br>循环头会告诉你“重复由什么控制”；循环体会告诉你“重复的动作是什么”。 | Example: `for score in scores:` means the same body runs once for each score.<br><br>例子：`for score in scores:` 表示同一段主体会为每个分数执行一次。 |
| **Ask how many times**<br><br>**它会执行几次** | One of the most important reading questions is: how many iterations happen?<br><br>读循环时最重要的问题之一是：它会执行几次？ | The number of iterations affects output, variable updates, and final results.<br><br>执行次数会影响输出、变量更新和最终结果。 | Example: `for i in range(5):` runs 5 times, not 4 and not forever.<br><br>例子：`for i in range(5):` 会执行 5 次，不是 4 次，也不是无限次。 |
| **Ask what changes each iteration**<br><br>**每轮什么会改变** | Most loops repeat a structure, but some values inside change every iteration.<br><br>大多数循环重复的是结构，但里面某些值会每轮改变。 | The loop variable, counters, totals, and current item often change each cycle.<br><br>循环变量、计数器、总数和当前项目常会在每次循环中变化。 | Example: In `for i in range(3):`, `i` becomes `0`, then `1`, then `2`.<br><br>例子：在 `for i in range(3):` 中，`i` 会依次变成 `0`、`1`、`2`。 |
| **Loop purpose**<br><br>**循环目的** | Loops are often used for traversal, counting, accumulation, filtering, or repeated prompting.<br><br>循环常用于遍历、计数、累加、筛选，或重复提示输入。 | Identifying the purpose makes the repeated actions easier to understand.<br><br>一旦识别出循环目的，就更容易理解里面重复做的事。 | Example: A loop that keeps asking until the user enters a valid choice has a validation purpose.<br><br>例子：一个不断要求输入直到用户给出合法选项的循环，目的就是验证输入。 |

# 10\. How to read functions / 怎样读函数

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Function Reading**<br><br>**读函数** | A function is a named block of reusable behavior.<br><br>函数是一段有名字、可重复使用的行为。 | To read a function well, identify its name, parameters, internal process, and return value.<br><br>要读懂函数，就要找出它的名字、参数、内部处理和返回值。 | Example: A function named `calculate_average(scores)` clearly suggests it computes an average from score data.<br><br>例子：名为 `calculate_average(scores)` 的函数，很明显是在根据分数数据计算平均值。 |
| **Function name tells purpose**<br><br>**函数名常揭示目的** | Good function names often reveal what the function is meant to do.<br><br>好的函数名通常会揭示它的目的。 | Verbs like `calculate`, `find`, `validate`, `load`, and `save` strongly indicate behavior type.<br><br>像 `calculate`、`find`、`validate`、`load`、`save` 这类动词，很强地暗示行为类型。 | Example: `validate_email(email)` tells you the function likely checks whether an email is valid.<br><br>例子：`validate_email(email)` 表示这个函数很可能是在检查邮箱是否有效。 |
| **Parameters tell required input**<br><br>**参数告诉你需要什么输入** | Function parameters tell you what data the function expects to receive.<br><br>函数参数告诉你这个函数要接收什么数据。 | Understanding parameters helps you see what the function depends on from outside.<br><br>理解参数，能帮助你看出函数从外部依赖什么。 | Example: If a function takes `items`, `target`, and `count`, it likely works with a collection, a goal value, and some limit or total.<br><br>例子：如果函数参数是 `items`、`target`、`count`，那它很可能是在处理一个集合、一个目标值，以及某个限制或总量。 |
| **Return value tells result**<br><br>**返回值告诉你产出** | The return value reveals what the function gives back after its work is done.<br><br>返回值会揭示函数做完工作后会交回什么。 | A return value may be a number, string, Boolean, list, dictionary, or object.<br><br>返回值可能是数字、字符串、布尔值、列表、字典或对象。 | Example: `return True` suggests validation success/failure logic; `return total` suggests accumulation result.<br><br>例子：`return True` 常表示验证成功/失败逻辑；`return total` 常表示累加结果。 |

# 11\. How to read code top-down and bottom-up / 怎样从上往下、从下往上读代码

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Top-down reading**<br><br>**从上往下读** | Top-down reading starts from the beginning and follows the intended program flow.<br><br>从上往下读，是从开头顺着程序的设计流程往下看。 | This is useful when code is small or follows a clear script-like structure.<br><br>当代码较小，或像脚本一样顺着执行时，这种方式很有用。 | Example: A short beginner Python program can often be understood top-down very effectively.<br><br>例子：一个短小的 Python 初学者程序，通常很适合直接从上往下读。 |
| **Bottom-up reading**<br><br>**从下往上找关键点** | Sometimes it helps to inspect important lines first, such as `return`, `print`, or final result blocks.<br><br>有时先看关键行更有帮助，例如 `return`、`print` 或结果区块。 | This helps reveal what the code is ultimately producing, which can clarify earlier steps.<br><br>这能先揭示代码最终产出了什么，从而反过来帮助理解前面的步骤。 | Example: In a function, reading the final `return` can tell you whether the function calculates, checks, or transforms something.<br><br>例子：在函数里，先看最后的 `return`，常能看出函数是在计算、检查还是转换。 |
| **Flexible reading**<br><br>**灵活读法** | Good code readers change reading strategy depending on the code shape and difficulty.<br><br>好的读代码者会根据代码形状和难度，调整读法。 | Sometimes you need top-down first, then trace one variable, then jump to a function definition, then return to the caller.<br><br>有时你会先从上往下，再追一个变量，再跳去函数定义，再回到调用处。 | Example: When a main program calls `process_data()`, you may jump into that function before continuing below the call line.<br><br>例子：主程序调用 `process_data()` 时，你可能会先跳进去看这个函数，再回来继续往下读。 |
| **Reading is navigation**<br><br>**读代码像导航** | Reading code is not always linear. It is often moving between related parts.<br><br>读代码不一定永远是线性的，经常需要在相关部分之间来回移动。 | You connect caller with callee, condition with branch, loop with body, and variable with updates.<br><br>你会把调用者和被调用函数、条件和分支、循环和主体、变量和更新连接起来。 | Example: To understand a function call, you may need to see both where it is called and how it is defined.<br><br>例子：要理解函数调用，你常常需要同时看它在哪里被调用、以及它是怎样被定义的。 |

# 12\. How to predict code before running it / 怎样在运行前预测代码

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Prediction**<br><br>**预测** | Strong code reading includes predicting behavior before execution.<br><br>强的读代码能力，包含在执行前先预测行为。 | Prediction forces you to mentally simulate the program and compare your expectation against real output later.<br><br>预测会逼你在脑中先模拟程序，再把想象结果和真实输出对比。 | Example: Before running a loop, guess the printed sequence first.<br><br>例子：运行循环前，先猜它会打印什么序列。 |
| **Mental execution**<br><br>**脑内执行** | You can mentally execute code by following values, branches, and loop iterations step by step.<br><br>你可以通过一步一步跟踪值、分支和循环轮次，在脑中执行代码。 | This process reveals whether you truly understand the code path or only think you do.<br><br>这个过程会暴露你是真的理解代码路径，还是只是“以为理解”。 | Example: If you predict wrong output, that is useful feedback about where your mental model is weak.<br><br>例子：如果你预测错输出，这其实是有价值的反馈，说明你哪块理解模型还不稳。 |
| **Use small examples first**<br><br>**先用小例子预测** | Prediction is easiest and most useful on short code or reduced examples first.<br><br>预测最适合从短代码或缩小版例子开始练。 | Small examples reduce complexity and train the core skill cleanly.<br><br>小例子能降低复杂度，更纯粹地训练这项能力。 | Example: Start with a 3-line loop instead of a 100-line program.<br><br>例子：先从 3 行的小循环开始，不要一上来就拿 100 行程序。 |
| **Compare prediction with reality**<br><br>**用现实结果对照预测** | The power of prediction comes from checking it against real execution.<br><br>预测的价值在于，把它和真实执行结果做对照。 | The gap between expectation and result reveals what needs correction.<br><br>“你以为会发生什么”和“实际发生了什么”之间的差距，就是你需要修正的地方。 | Example: You predicted 5 iterations, but it ran 4 times; now you inspect the `range` boundaries more carefully.<br><br>例子：你以为会执行 5 次，结果只跑了 4 次，那就说明你要更仔细看 `range` 的边界。 |

# 13\. How to read long code without getting lost / 怎样读长代码不迷路

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Chunking**<br><br>**分块阅读** | Long code should be broken into chunks, not attacked as one giant wall.<br><br>长代码要分块读，不能把它当一整面墙硬撞。 | Divide the code into sections such as imports, setup, helper functions, main logic, and output or cleanup.<br><br>把代码拆成导入、初始化、辅助函数、主逻辑、输出或收尾等部分。 | Example: A file may have 5 helper functions and 1 main execution block; read each piece separately first.<br><br>例子：一个文件可能有 5 个辅助函数和 1 个主执行区，你应该先分开看。 |
| **Mark landmarks**<br><br>**找地标** | In long code, find landmarks that help orient you.<br><br>长代码里要找“地标”，帮助自己定位。 | Landmarks include function definitions, class definitions, loops, condition blocks, comments, and key variable declarations.<br><br>地标包括函数定义、类定义、循环、条件区块、注释和关键变量声明。 | Example: In a data-processing script, one landmark might be the function that loads data, another the function that cleans it, another the function that saves output.<br><br>例子：在数据处理脚本中，一个地标可能是加载数据的函数，另一个是清理数据的函数，再一个是保存结果的函数。 |
| **Follow one thread at a time**<br><br>**一次追一条线** | Do not try to understand every relationship at once in long code.<br><br>读长代码时，不要试图一次看懂所有关系。 | Follow one thread, such as one variable, one function call chain, or one output path, then return and trace another thread.<br><br>一次先追一条线，比如一个变量、一条函数调用链，或一条输出路径；看完再回来追别的。 | Example: First trace where `user_data` is created and modified; later trace how it is displayed or saved.<br><br>例子：先追 `user_data` 在哪里创建和修改，再回来追它如何被显示或保存。 |
| **Summarize as you go**<br><br>**边读边总结** | Summarizing each block in your own words prevents overload.<br><br>边读边用自己的话总结每个区块，可以防止信息过载。 | A short summary forces understanding and creates a map in memory.<br><br>短总结会逼你理解，也会在脑中建立地图。 | Example: “This function checks input validity.” “This loop accumulates total sales.”<br><br>例子：“这个函数负责检查输入是否合法。” “这个循环负责累计总销售额。” |

# 14\. How comments and naming help code reading / 注释和命名怎样帮助读代码

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Meaningful Names**<br><br>**有意义的命名** | Good names reduce the amount of guessing needed while reading.<br><br>好的命名会减少读代码时需要猜测的程度。 | Names can reveal purpose, data meaning, and expected behavior before you inspect full logic.<br><br>名字本身就能在你看完整逻辑前，先透露目的、数据意义和预期行为。 | Example: `monthly_sales_total` is easier to understand than `x`.<br><br>例子：`monthly_sales_total` 比 `x` 更容易理解。 |
| **Comments as guidance**<br><br>**注释作为引导** | Good comments explain intent, not obvious syntax.<br><br>好的注释解释的是“意图”，不是显而易见的语法。 | Intent comments help readers understand why code exists, especially when the reason is not obvious from syntax alone.<br><br>意图型注释能帮助读者明白代码“为什么存在”，尤其是当语法本身看不出原因时。 | Example: `# Skip empty lines before processing` is more useful than `# if line == ""`.<br><br>例子：`# Skip empty lines before processing` 会比 `# if line == ""` 更有帮助。 |
| **Poor naming hurts reading**<br><br>**差命名会严重伤害阅读** | Bad names force the reader to reverse-engineer the role of every variable and function.<br><br>差的命名会逼读者反向推理每个变量和函数的作用。 | This increases mental load and makes bugs harder to spot.<br><br>这会增加大脑负担，也让 bug 更难被发现。 | Example: `a`、`b`、`temp1`、`data2` are often weak names unless the context is extremely simple.<br><br>例子：`a`、`b`、`temp1`、`data2` 通常是很弱的命名，除非上下文非常简单。 |
| **Comments are not a replacement**<br><br>**注释不是替代品** | Comments help, but they cannot fully save badly structured code.<br><br>注释有帮助，但它不能完全拯救结构很差的代码。 | If code is clear, comments support it; if code is confusing, comments may only partly reduce confusion.<br><br>如果代码本身清楚，注释是辅助；如果代码本身混乱，注释最多只能部分减轻痛苦。 | Example: A clear function with a clear name often needs fewer comments than messy code with many comments.<br><br>例子：一个名字清楚的清晰函数，通常比一堆乱代码更不需要大量注释。 |

# 15\. How to read code you do not understand at first / 怎样读一开始看不懂的代码

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Do not panic**<br><br>**先别慌** | Not understanding code immediately is normal, especially if the code is new, long, or uses unfamiliar concepts.<br><br>一开始看不懂代码很正常，尤其是代码很新、很长，或用了你不熟的概念。 | Panic blocks reasoning. Calm inspection keeps the mind open to patterns and clues.<br><br>慌张会阻断推理；冷静检查会让大脑继续寻找模式和线索。 | Example: Seeing `enumerate`、`zip` 或推导式 for the first time does not mean the whole program is beyond you.<br><br>例子：第一次看到 `enumerate`、`zip` 或推导式，不代表整个程序都超出你的能力。 |
| **Find the unfamiliar piece**<br><br>**找出真正陌生的点** | Often the whole program is not confusing; only one or two constructs are unfamiliar.<br><br>很多时候，不是整个程序都难，而是其中一两个结构你不认识。 | Isolating the unknown part reduces fear and makes the learning task concrete.<br><br>把陌生点单独找出来，会降低恐惧，也让学习任务更具体。 | Example: You may understand the loop and condition, but not the dictionary method being used.<br><br>例子：你可能其实懂循环和条件，只是不懂某个字典方法。 |
| **Reduce to a smaller example**<br><br>**缩成更小例子** | If the original code is too complex, rewrite the same pattern in a smaller example.<br><br>如果原代码太复杂，就把同样模式改写成更小的例子。 | Smaller examples expose the core mechanism more clearly than the original full version.<br><br>更小的例子会比原来的完整版本更清楚地暴露核心机制。 | Example: If a nested loop is confusing in a big program, recreate it with a tiny 2x2 list example.<br><br>例子：如果大程序里的嵌套循环很乱，就用一个小小的 2x2 列表重做一次。 |
| **Return after learning**<br><br>**学会小点后再回原代码** | Once you understand the small missing concept, return to the original code and reread it.<br><br>当你补懂了那个小缺口后，再回去重新读原代码。 | The program often becomes much clearer after one missing prerequisite is fixed.<br><br>很多时候，只要补上一个前置概念，整段程序就会清楚很多。 | Example: Learning `items()` may suddenly make a dictionary loop understandable.<br><br>例子：一旦懂了 `items()`，一个字典循环可能会突然变得简单。 |

```markdown
# 16\. Complete Practical Example 1 / 完整实际例子 1

下面先看一个很短的程序。  
目标不是只看懂语法，而是学会 **怎么读**。

## Example Code

```python
scores = [70, 85, 90, 60]
total = 0

for score in scores:
    total += score

average = total / len(scores)
print("Average:", average)
```

## How to read it properly / 正确读法

| **Step**<br><br>**步骤** | **English** | **中文** |
| --- | --- | --- |
| 1 | First identify the goal: this program calculates an average from a list of scores. | 先找目标：这个程序是在根据一组分数计算平均值。 |
| 2 | Identify the input data: `scores` is the starting data. | 找输入数据：`scores` 是起始数据。 |
| 3 | Identify the accumulator: `total = 0` shows `total` will be built over time. | 找累加器：`total = 0` 表示 `total` 会随着时间逐步累加。 |
| 4 | Read the loop: `for score in scores:` means each score will be visited once. | 读循环：`for score in scores:` 表示每个分数都会被访问一次。 |
| 5 | Trace variable change: `total += score` updates `total` every iteration. | 追踪变量变化：`total += score` 表示每一轮 `total` 都会更新。 |
| 6 | Read the final processing line: `average = total / len(scores)` uses sum and count to compute average. | 读最终处理行：`average = total / len(scores)` 用总和和数量来算平均值。 |
| 7 | Read output: `print("Average:", average)` displays the result. | 读输出：`print("Average:", average)` 把结果显示出来。 |

## Trace Table / 追踪表

| **Iteration**<br><br>**轮次** | **score**<br><br>**当前值** | **total before**<br><br>**更新前** | **total after**<br><br>**更新后** |
| --- | --- | --- | --- |
| 1 | 70 | 0 | 70 |
| 2 | 85 | 70 | 155 |
| 3 | 90 | 155 | 245 |
| 4 | 60 | 245 | 305 |

最后：

- `total = 305`
- `len(scores) = 4`
- `average = 305 / 4 = 76.25`

# 17\. Complete Practical Example 2 / 完整实际例子 2

## Example Code

```python
age = 16

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

## How to read it properly / 正确读法

| **Step**<br><br>**步骤** | **English** | **中文** |
| --- | --- | --- |
| 1 | Identify the goal: the code classifies a person by age. | 先找目标：这段代码是在根据年龄分类一个人。 |
| 2 | Identify the key variable: `age` is the data used for decision-making. | 找关键变量：`age` 是做判断的数据。 |
| 3 | Read the condition as a question: “Is age at least 18?” | 把条件读成问题：“age 是否至少 18？” |
| 4 | Evaluate the answer: with `age = 16`, the condition is false. | 评估答案：因为 age = 16，这个条件是假的。 |
| 5 | Choose the branch: because the condition is false, the else block runs. | 选择分支：因为条件是假，所以执行 else 区块。 |
| 6 | Determine output: the result printed is Minor. | 确定输出：最终打印的是 Minor。 |

# 18\. Complete Practical Example 3 / 完整实际例子 3

## Example Code

```python
def find_max(a, b):
    if a > b:
        return a
    else:
        return b

result = find_max(8, 5)
print(result)
```

## How to read it properly / 正确读法

| **Step**<br><br>**步骤** | **English** | **中文** |
| --- | --- | --- |
| 1 | Start with the function name: find_max suggests finding the larger of two values. | 先看函数名：find_max 暗示这是找两个值里较大的那个。 |
| 2 | Read the parameters: a and b are the two values the function compares. | 看参数：a 和 b 是被比较的两个值。 |
| 3 | Read the condition: “Is a greater than b?” | 读条件：“a 是否大于 b？” |
| 4 | Read each return branch: if true, return a; otherwise return b. | 读两个返回分支：如果真，返回 a；否则返回 b。 |
| 5 | Read the call site: find_max(8, 5) means a = 8, b = 5. | 读调用位置：find_max(8, 5) 表示 a = 8，b = 5。 |
| 6 | Evaluate the result: since 8 > 5 is true, the function returns 8. | 评估结果：因为 8 > 5 为真，所以函数返回 8。 |
| 7 | Read the final output: print(result) prints 8. | 读最终输出：print(result) 会打印 8。 |

# 19\. Self-Check Table / 自我检查表

| **Question (English)**<br><br>**英文问题** | **中文问题** |
| --- | --- |
| Can you explain what the program is trying to do before reading every line? | 你能不能在逐行读之前，先说出程序想做什么？ |
| Can you identify input, processing, condition, loop, and output blocks? | 你能不能分辨输入、处理、判断、循环和输出区块？ |
| Can you trace how a variable changes from beginning to end? | 你能不能追踪一个变量从头到尾怎样变化？ |
| Can you read an `if` condition as a question? | 你能不能把 if 条件读成一个问题？ |
| Can you tell how many times a loop runs and what changes in each iteration? | 你能不能判断循环会跑几次，以及每轮改变什么？ |
| Can you explain a function using its name, parameters, and return value? | 你能不能用函数名、参数和返回值去解释一个函数？ |
| Can you summarize each code block in one sentence? | 你能不能用一句话总结每个代码块？ |

# 20\. Key Takeaways / 本课重点总结

| **Type**<br><br>**类型** | **Core Idea**<br><br>**核心概念** | **How it works**<br><br>**它如何运作** | **Usage / Example**<br><br>**用途 / 例子** |
| --- | --- | --- | --- |
| **Read for purpose**<br><br>**为目的而读** | Always begin by asking what the code is meant to achieve.<br><br>读代码时，永远先问它想达成什么。 | Purpose organizes all later details.<br><br>目的会组织后面的所有细节。 | Example: "This code searches for a value."<br><br>例子："这段代码是在找一个值。" |
| **Read by structure**<br><br>**按结构读** | Python code should be read by blocks and indentation, not only by single lines.<br><br>Python 代码要按区块和缩进来读，不只是按单行读。 | Structure shows relationships between parts.<br><br>结构会显示各部分的关系。 | Example: An indented block belongs to a loop, function, or condition.<br><br>例子：一个缩进区块属于某个循环、函数或条件。 |
| **Trace data flow**<br><br>**追踪数据流** | Understanding code requires following how data enters, changes, and leaves.<br><br>理解代码必须追踪数据怎样进入、怎样改变、怎样离开。 | Variables carry the state of the program.<br><br>变量承载程序状态。 | Example: input → variable → loop → result → print.<br><br>例子：输入 → 变量 → 循环 → 结果 → 输出。 |
| **Prediction improves reading**<br><br>**预测会加强阅读能力** | Predicting output before running helps reveal real understanding.<br><br>运行前先预测输出，能更真实地暴露理解程度。 | Mental simulation strengthens logic.<br><br>脑内模拟会强化逻辑能力。 | Example: Guess a loop's output first, then run it.<br><br>例子：先猜循环输出，再运行验证。 |
| **Confusion should be reduced, not feared**<br><br>**困惑要被缩小，不是被害怕** | When code feels hard, isolate the unknown part and simplify it.<br><br>当代码很难时，要把陌生部分拆出来并简化。 | Small understanding steps build full understanding later.<br><br>小理解会慢慢叠成完整理解。 | Example: Learn one unfamiliar method, then return to the whole program.<br><br>例子：先补懂一个陌生方法，再回去看整个程序。 |
```
