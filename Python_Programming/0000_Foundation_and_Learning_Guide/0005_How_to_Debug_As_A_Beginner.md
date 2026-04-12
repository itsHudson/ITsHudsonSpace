# 1\. What debugging really means / 什么才叫真正的 Debug

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Debugging 调试** | Debugging means finding, understanding, and fixing problems in code. <br>调试，指的是找出、理解并修正代码中的问题。 | You compare what the program actually does with what you expected it to do, then locate the reason for the mismatch. <br>你会把"程序实际做了什么"和"你预期它该做什么"进行对比，然后找出差异产生的原因。 | Example: You expected the program to print Pass, but it printed Fail, so you inspect the condition and the input value. <br>例子：你原本预期程序打印 Pass，结果它打印了 Fail，于是你去检查条件和输入值。 |
| **Debugging is normal 调试是正常过程** | Bugs do not mean you are bad at programming. They mean programming is happening. <br>有 bug 不代表你不行，而是代表你真的在做编程。 | Every non-trivial program contains moments where logic, syntax, data, or assumptions do not match reality. <br>任何稍微复杂一点的程序，都会出现逻辑、语法、数据或假设和现实不一致的时刻。 | Example: Even a simple input program may fail if the user enters text when the code expected a number. <br>例子：即使是简单输入程序，如果用户输入文字而代码预期数字，也会出错。 |
| **Debugging is reasoning 调试是一种推理** | Debugging is not random guessing. It is logical investigation. <br>调试不是乱猜，而是一种逻辑调查。 | You inspect clues: error type, line number, variable values, program flow, conditions, loops, and outputs. <br>你会检查线索：错误类型、行号、变量值、程序流程、条件、循环和输出。 | Example: Instead of randomly rewriting ten lines, you first inspect where the value became wrong. <br>例子：你不会随便重写十行代码，而是先检查值是从哪里开始变错的。 |
| **Debugging builds skill 调试会建立能力** | Each bug you fix improves your understanding of how code works. <br>每修好一个 bug，你对代码如何运作的理解都会提升。 | Bugs force you to inspect details you might otherwise ignore, such as type conversion, variable updates, or condition boundaries. <br>bug 会逼你看清一些你本来会忽略的细节，例如类型转换、变量更新或条件边界。 | Example: After fixing enough TypeError bugs, you become much more aware of string vs integer operations. <br>例子：修多了 TypeError 以后，你会更敏感地意识到字符串和整数运算的区别。 |

# 2\. Why beginners panic when code breaks / 为什么初学者一出错就慌

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Too many unknowns 未知太多** | Beginners panic because one error feels like many possible problems at once. <br>初学者会慌，是因为一个错误看起来像同时有很多种可能。 | When syntax, logic, input, variables, and output are all still new, a single bug can feel overwhelming. <br>当语法、逻辑、输入、变量和输出都还不稳时，一个 bug 就会显得非常巨大。 | Example: A simple ValueError may feel terrifying if you are still not comfortable with input() and type conversion. <br>例子：如果你对 input() 和类型转换还不熟，一个简单的 ValueError 都会显得很可怕。 |
| **They read red text emotionally 他们用情绪看红字** | Many beginners see an error message and emotionally translate it as "I failed." <br>很多初学者一看到错误信息，情绪上就会把它翻译成"我失败了"。 | This emotional reaction blocks careful reading and makes the bug feel bigger than it is. <br>这种情绪反应会阻碍冷静阅读，也会把 bug 放大。 | Example: Instead of reading the traceback, the learner scrolls away, copies random code, or gives up immediately. <br>例子：学习者没有仔细读 traceback，而是立刻乱改代码、去抄答案，或者直接放弃。 |
| **They expect perfect first attempts 他们期待第一版就完美** | Beginners often expect working code immediately, which is unrealistic. <br>初学者常常期待代码第一次就完美运行，这其实不现实。 | When the first version fails, they interpret the failure as evidence of inability instead of a normal development step. <br>当第一版失败时，他们会把它理解成"自己不行"，而不是"这是开发中的正常步骤"。 | Example: A beginner writes a loop once, gets wrong output, and concludes "I do not understand loops at all." <br>例子：初学者写了一次循环，结果输出不对，就直接得出"我完全不懂循环"的结论。 |
| **They do not yet have a debug method 他们还没有调试流程** | Panic is stronger when you do not know what steps to follow. <br>如果你不知道应该按什么步骤检查，慌张就会更强。 | A clear debug method reduces chaos because it gives the brain an order of actions. <br>一个清楚的调试流程能减少混乱，因为它会给大脑一个可执行的顺序。 | Example: Knowing "read the error → find the line → inspect values → test a smaller part" is calming because it turns panic into action. <br>例子：知道"先读错误 → 找到行号 → 检查值 → 测小部分"会让人冷静，因为恐慌会变成行动。 |

# 3\. The three main kinds of bugs / 三种最主要的 bug

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Syntax Error 语法错误** | A syntax error means Python could not understand the structure of your code. <br>语法错误表示 Python 无法理解你的代码结构。 | The code fails before normal execution because the written structure breaks Python's grammar rules. <br>代码通常在正常执行前就失败，因为写出来的结构违反了 Python 的语法规则。 | Example: Missing colon after if, bad indentation, unclosed parenthesis. <br>例子：if 后少冒号、缩进错误、括号没关。 |
| **Runtime Error 运行时错误** | A runtime error means the code started running, but crashed during execution. <br>运行时错误表示代码已经开始运行，但在执行过程中崩掉了。 | Python understood the syntax, but when actual values or states appeared, something invalid happened. <br>Python 虽然看懂了语法，但在真实值或状态出现时，发生了无效操作。 | Example: Dividing by zero, converting invalid text to integer, accessing a missing key, index out of range. <br>例子：除以零、把非法文字转整数、访问不存在的键、索引越界。 |
| **Logic Error 逻辑错误** | A logic error means the code runs without crashing, but the result is wrong. <br>逻辑错误表示代码能运行，但结果不正确。 | The structure is valid and execution completes, but the instructions do not match the intended logic. <br>结构是合法的，执行也能结束，但你的指令逻辑不符合真正目标。 | Example: Average is calculated with the wrong divisor, condition uses > instead of >=, total is reset inside the loop by mistake. <br>例子：平均值用错除数、条件把 >= 写成 >、在循环里错误地重置 total。 |

# 4\. How to recognize each bug type quickly / 怎样快速分辨每种 bug

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Syntax Error Clue 语法错误线索** | If the code does not even start properly, think syntax first. <br>如果代码连正常开始都做不到，先怀疑语法。 | Python usually points near the place where structure broke, though sometimes the real cause may be slightly earlier. <br>Python 通常会指向结构坏掉附近的位置，不过真正原因有时可能稍微更前面一点。 | Example: SyntaxError: invalid syntax or indentation-related messages appear before meaningful output happens. <br>例子：SyntaxError: invalid syntax 或缩进相关信息会在程序真正输出之前就出现。 |
| **Runtime Error Clue 运行时错误线索** | If the program starts but crashes while running, think runtime error. <br>如果程序已经开始，但运行到中途崩掉，先怀疑运行时错误。 | A traceback usually shows the error type and the exact place where invalid execution happened. <br>traceback 通常会显示错误类型，以及无效执行发生的具体位置。 | Example: The program prints one line, then crashes on int(input(...)) because the user entered abc. <br>例子：程序先打印了一行，然后在 int(input(...)) 崩掉，因为用户输入了 abc。 |
| **Logic Error Clue 逻辑错误线索** | If the program runs fully but produces the wrong answer, think logic error. <br>如果程序完整跑完了，但答案不对，先怀疑逻辑错误。 | You compare expected output with actual output, then trace where reasoning diverged. <br>你会把预期输出和真实输出对比，然后追踪逻辑是从哪里开始偏掉的。 | Example: Program says a score of 50 is Fail even though the requirement says 50 should pass. <br>例子：程序把 50 分判成 Fail，但题目要求 50 应该及格。 |
| **Mixed Bugs 混合错误** | Sometimes one bug hides another, so fixing one may reveal the next. <br>有时一个 bug 会遮住另一个，所以修完一个之后，下一个才会出现。 | This is normal because the program may have multiple issues layered together. <br>这很正常，因为程序可能有多层问题叠在一起。 | Example: First fix the missing colon, then the code runs and reveals a NameError that was hidden before. <br>例子：先修掉少了的冒号，程序开始运行后，才暴露出原本被挡住的 NameError。 |

# 5\. The first rule of beginner debugging / 初学者调试第一原则

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Do not guess wildly 不要乱猜** | The first rule is: do not make random changes everywhere. <br>第一原则是：不要到处乱改。 | Random edits destroy clues and make it harder to know which change caused which effect. <br>乱改会破坏线索，也会让你不知道到底是哪次改动造成了什么影响。 | Example: If a loop output is wrong, do not rewrite the whole file immediately; inspect the loop logic first. <br>例子：如果循环输出错了，不要立刻重写整个文件；先检查循环逻辑。 |
| **One change at a time 一次只改一个点** | Good debugging isolates changes. <br>好的调试会隔离改动。 | If you change one thing and retest, you learn whether that change helped or not. <br>如果你一次只改一个点再测试，你就能知道这次改动到底有没有帮助。 | Example: First fix the condition, run again, then if still wrong inspect the loop count next. <br>例子：先改条件，再运行；如果还是不对，再去检查循环次数。 |
| **Read before changing 先读，再改** | The code is evidence. You must inspect the evidence before acting. <br>代码是证据；你必须先看证据，再采取行动。 | Reading the error, the variable states, and the surrounding lines often reveals much more than blind rewriting. <br>阅读错误、变量状态和附近几行，往往比盲目重写更有用。 | Example: A NameError can often be fixed by checking spelling and where the variable was defined, without touching unrelated code. <br>例子：NameError 常常只要检查拼写和变量定义位置就能修好，不需要碰其他无关代码。 |
| **Stay mechanical, not emotional 用流程，不用情绪** | Good debugging is calm and mechanical. <br>好的调试是冷静且机械化的。 | When you follow a method, the bug becomes a puzzle instead of a personal attack. <br>当你遵循流程时，bug 会变成一道谜题，而不是对你的攻击。 | Example: "What is the error type? What line? What value caused it?" is much better than "Why does this always happen to me?" <br>例子："错误类型是什么？哪一行？哪个值引发的？"会比"为什么总是我这么倒霉？"有效得多。 |

# 6\. The basic beginner debug workflow / 初学者最基础的调试流程

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Step 1: Reproduce the problem 第一步：重现问题** | Confirm that the bug really happens and know exactly when it happens. <br>先确认问题真的会发生，并知道它是在什么情况下发生。 | You rerun the code with the same inputs or steps and observe the failure carefully. <br>你用相同输入或相同步骤重新运行代码，并仔细观察失败。 | Example: "The crash happens only when I enter text instead of a number." <br>例子："只有当我输入文字而不是数字时，程序才会崩。" |
| **Step 2: Read the error or wrong result 第二步：读错误或读错结果** | Look at what Python or the output is telling you. <br>看 Python 或输出到底告诉了你什么。 | Error type, line number, and actual output are clues, not noise. <br>错误类型、行号和真实输出都是线索，不是噪音。 | Example: ValueError tells you the issue is not missing syntax, but invalid value conversion. <br>例子：ValueError 表示问题不是语法缺失，而是值转换不合法。 |
| **Step 3: Narrow the location 第三步：缩小位置** | Identify the smallest relevant area of code related to the problem. <br>找出和问题最相关的最小代码范围。 | This prevents you from mentally handling too much code at once. <br>这会防止你一次处理过多代码。 | Example: If the wrong output starts after the loop, focus on the loop and the final computation, not the unrelated menu code. <br>例子：如果错结果出现在循环之后，就先看循环和最终计算，不要分心去看无关菜单代码。 |
| **Step 4: Inspect values 第四步：检查值** | Check what the important variables contain at the critical moment. <br>检查关键变量在关键时刻里面到底装了什么值。 | Many bugs become obvious once you see real variable values instead of assumed values. <br>很多 bug 一旦看到变量的真实值，而不是你脑中假设的值，就会变得明显。 | Example: You expected count = 5, but print shows it is actually 0 because it was reset inside the loop. <br>例子：你以为 count = 5，但 print 告诉你其实是 0，因为它在循环里被重置了。 |
| **Step 5: Change one thing and retest 第五步：改一处，再重测** | Make one targeted fix, then run the code again. <br>做一个有针对性的修正，然后重新运行。 | This reveals whether your hypothesis about the bug was correct. <br>这会验证你对 bug 的假设是否正确。 | Example: Change > to >=, rerun, and confirm whether score 50 is now classified correctly. <br>例子：把 > 改成 >=，重新运行，看看 50 分现在是否被正确分类。 |
| **Step 6: Verify the fix 第六步：验证修复** | Do not stop just because the code runs once. Confirm the fix under a few cases. <br>不要因为代码跑过一次就停下，要用几个案例确认修复。 | A fix is trustworthy only if it handles relevant normal and edge cases too. <br>只有当修复也能处理正常情况和边界情况时，它才值得信任。 | Example: After fixing a pass/fail condition, test 49, 50, and 51. <br>例子：修好及格判断后，测试 49、50、51。 |

# 7\. How to read a traceback / 怎样看 traceback

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Traceback is a clue trail traceback 是线索轨迹** | A traceback is Python showing the path to the crash. <br>traceback 是 Python 展示崩溃路径的方式。 | It usually includes the file, line number, and error type, and sometimes a chain of function calls leading to the failure. <br>它通常会包含文件、行号、错误类型，有时还会包含导致失败的一连串函数调用路径。 | Example: If main() calls convert_input(), and that function crashes, the traceback may show both locations. <br>例子：如果 main() 调用了 convert_input()，而后者崩掉，traceback 可能会同时显示两个位置。 |
| **Read the error type 先读错误类型** | The error type tells you what kind of failure happened. <br>错误类型会告诉你这是哪一类失败。 | Types like NameError, TypeError, ValueError, IndexError, and KeyError narrow your search direction immediately. <br>NameError、TypeError、ValueError、IndexError、KeyError 等类型，会立刻缩小你的搜索方向。 | Example: IndexError means the code tried to access a position that does not exist in the sequence. <br>例子：IndexError 表示代码尝试访问序列中不存在的位置。 |
| **Read the line number 读行号** | The line number tells you where Python noticed the problem. <br>行号会告诉你 Python 在哪里注意到问题。 | Sometimes the exact cause is on that line; sometimes the line only reveals the effect of an earlier bad value or assumption. <br>有时真正原因就在那一行；有时那一行只是暴露了前面更早就出问题的值或假设。 | Example: The crash line may be print(items\[5\]), but the deeper issue is that the list has only 3 items because input collection failed earlier. <br>例子：崩溃行可能是 print(items\[5\])，但更深层原因是列表其实只有 3 个元素，因为前面的输入收集失败了。 |
| **Read the message text 读错误说明文字** | The message text often explains what Python expected and what it found instead. <br>错误说明文字通常会解释 Python 原本预期什么，以及它实际看到了什么。 | This can reveal whether the issue is missing data, wrong type, invalid value, or unsupported operation. <br>这能帮助你判断问题是缺数据、类型错误、值不合法，还是操作不被支持。 | Example: invalid literal for int() strongly suggests a text-to-integer conversion problem. <br>例子：invalid literal for int() 非常明确地暗示这是文字转整数的问题。 |

# 8\. Common beginner error types and what they usually mean / 初学者常见错误类型，以及它们通常代表什么

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **NameError** | A name was used before being defined, or the spelling is wrong. <br>某个名字在定义前就被使用，或者拼写错了。 | Python looks for the variable or function name and cannot find a valid matching definition in scope. <br>Python 去找变量或函数名，但在当前作用域里找不到对应定义。 | Example: pritn("Hello") or using total before assigning it. <br>例子：pritn("Hello")，或者在赋值前就使用 total。 |
| **TypeError** | An operation used incompatible data types or the wrong kind of object behavior. <br>某个操作使用了不兼容的数据类型，或对象行为类型不对。 | Python understood the syntax, but the operation itself makes no sense for the involved types. <br>Python 虽然看懂了语法，但这个操作对相关类型来说没有意义。 | Example: "5" + 3, or calling len(10). <br>例子："5" + 3，或者 len(10)。 |
| **ValueError** | The type is acceptable, but the actual value is not valid for the requested operation. <br>类型本身可以，但值本身不合法。 | A conversion or operation receives data in the wrong format or impossible form. <br>转换或某操作拿到了格式不对或不可能处理的数据。 | Example: int("abc"). <br>例子：int("abc")。 |
| **IndexError** | A sequence index is outside the valid range. <br>序列索引超出了合法范围。 | The program asked for a position that does not exist in a list, string, or tuple. <br>程序去访问列表、字符串或元组中不存在的位置。 | Example: Accessing items\[10\] when the list has only 3 items. <br>例子：列表只有 3 个元素，却访问 items\[10\]。 |
| **KeyError** | A dictionary key was requested, but it does not exist. <br>字典里请求了一个不存在的键。 | The program assumes a key is present when it is not actually present in the dictionary. <br>程序以为某个键存在，但它其实并不在字典里。 | Example: student\["age"\] when "age" is not in the dictionary. <br>例子：student\["age"\]，但字典里没有 "age"。 |
| **ZeroDivisionError** | The program tried to divide by zero. <br>程序尝试除以零。 | This often appears when a count, total, or denominator becomes zero unexpectedly. <br>这种错误常出现在计数器、总量或分母意外变成 0 的时候。 | Example: average = total / count when count == 0. <br>例子：average = total / count，但 count == 0。 |
| **IndentationError** | Python expected a certain indentation structure but did not find it. <br>Python 预期某种缩进结构，却没有找到。 | Because indentation defines code blocks in Python, inconsistent or missing indentation breaks structure. <br>因为缩进在 Python 里定义代码区块，不一致或缺失缩进会直接破坏结构。 | Example: Forgetting to indent the body under if or for. <br>例子：忘记给 if 或 for 下面的主体缩进。 |

# 9\. How to debug syntax errors / 怎样调试语法错误

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Read near the reported line 看报错附近** | For syntax errors, the reported line is often close to the real issue. <br>对语法错误来说，报错行通常离真正问题很近。 | The parser becomes confused where structure breaks, so inspect that line and the few lines before it. <br>语法分析器会在结构坏掉的地方变得混乱，所以要检查该行和前面几行。 | Example: A missing closing parenthesis on line 5 may cause a syntax complaint on line 6. <br>例子：第 5 行少了一个右括号，可能会让第 6 行报语法错。 |
| **Check punctuation 检查标点结构** | Missing or misplaced punctuation is a very common syntax issue. <br>漏掉或放错标点，是非常常见的语法问题。 | Colons, parentheses, brackets, braces, and quotes all create structure that must be completed correctly. <br>冒号、括号、中括号、大括号和引号都会形成结构，必须正确闭合。 | Example: Forgetting the colon in if score > 50: will cause a syntax error. <br>例子：if score > 50: 少了冒号就会触发语法错误。 |
| **Check indentation 检查缩进** | In Python, indentation errors are structure errors, not mere style issues. <br>在 Python 里，缩进错不是风格问题，而是结构问题。 | Python uses indentation to know what belongs inside a loop, condition, or function. <br>Python 依靠缩进来判断哪些代码属于循环、条件或函数内部。 | Example: If the body under for is not indented, the loop structure is broken. <br>例子：如果 for 下面的主体没有缩进，循环结构就坏了。 |
| **Simplify the line 简化问题行** | If a complex line causes syntax confusion, simplify it to isolate the structure issue. <br>如果复杂语句导致语法混乱，就把它简化，以隔离结构问题。 | Smaller, simpler syntax is easier to inspect than one overloaded expression. <br>更小、更简单的语法，比一个过载的大表达式更容易检查。 | Example: Break a long nested function call into several simple assignments. <br>例子：把很长的嵌套函数调用拆成几个简单赋值。 |

# 10\. How to debug runtime errors / 怎样调试运行时错误

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Look at the real values 看真实值** | Runtime errors usually happen because real values differ from what you assumed. <br>运行时错误通常发生在"真实值"和"你假设的值"不一致的时候。 | Inspect the variables involved in the crashing line and determine what they actually contain at runtime. <br>检查出错行涉及的变量，确定它们在运行时真正装着什么。 | Example: If int(user_input) crashes, print user_input first to see what text was actually entered. <br>例子：如果 int(user_input) 崩掉，先打印 user_input 看用户到底输入了什么。 |
| **Check program state 检查程序状态** | Some runtime errors depend not only on one value, but on the state built earlier in the program. <br>有些运行时错误不只和一个值有关，还和程序前面建立出的状态有关。 | A list may be empty, a dictionary may lack a key, or a file may not exist because of earlier logic decisions. <br>列表可能为空、字典可能没有键、文件可能不存在，而这些都可能是前面逻辑造成的。 | Example: numbers\[0\] fails not because indexing is "bad," but because the list is empty at that moment. <br>例子：numbers\[0\] 失败不是因为索引本身"坏了"，而是因为那一刻列表是空的。 |
| **Reproduce the crash reliably 稳定重现崩溃** | You should know exactly what input or path causes the runtime error. <br>你应该知道到底是什么输入或什么执行路径会导致运行时错误。 | Reliable reproduction helps you test whether the fix truly works later. <br>稳定重现能帮助你之后验证修复是否真的有效。 | Example: "This only crashes when count is 0." <br>例子："这个程序只有在 count 是 0 的时候才会崩。" |
| **Guard dangerous operations 保护危险操作** | Many runtime errors can be prevented by validation before the dangerous operation happens. <br>很多运行时错误，都可以通过在危险操作前先做验证来预防。 | Validation checks assumptions such as non-empty data, valid format, non-zero divisors, or existing keys. <br>验证会检查一些假设，例如数据非空、格式合法、分母非零或键存在。 | Example: Check if count != 0: before dividing by count. <br>例子：在除以 count 前，先检查 if count != 0:。 |

# 11\. How to debug logic errors / 怎样调试逻辑错误

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Logic errors require comparison 逻辑错误要靠对比发现** | Logic errors are found by comparing expected behavior with actual behavior. <br>逻辑错误要通过"预期行为"和"实际行为"的对比来发现。 | Because the code still runs, you need test cases and reasoning rather than crash messages. <br>因为代码还能运行，所以你需要测试案例和推理，而不是靠崩溃信息。 | Example: If the largest number function returns 5 when the input contains 9, your code ran, but your logic is wrong. <br>例子：如果找最大值函数在输入里明明有 9，却返回 5，那代码能跑，但逻辑错了。 |
| **Use small test cases 用小测试案例** | Small controlled inputs make logic easier to inspect. <br>小而可控的输入，会让逻辑更容易被检查。 | Simple data reduces mental load and shows exactly where the reasoning diverges. <br>简单数据会降低思考负担，也更容易看清逻辑是从哪里偏掉的。 | Example: Test a sorting idea with \[3, 1, 2\] before trying a large messy list. <br>例子：先用 \[3, 1, 2\] 测排序逻辑，而不是一开始就用很大的复杂列表。 |
| **Trace each step 逐步追踪** | For logic bugs, trace the code step by step and record important variable changes. <br>对逻辑 bug，要逐步追踪代码并记录关键变量变化。 | Logic errors are often invisible until you follow the computation over time. <br>逻辑错误常常只有在你跟着计算一步一步走时才会显现。 | Example: If a total is wrong, track the total after each loop iteration. <br>例子：如果 total 错了，就记录每轮循环后的 total。 |
| **Check boundaries 检查边界** | Many logic bugs come from edge cases and boundaries. <br>很多逻辑 bug 都来自边界情况。 | Conditions like >, >=, <, <=, first/last item handling, and empty data cases often create mistakes. <br>像 >、>=、<、<=、首项/末项处理、空数据这些边界点，最容易产生错误。 | Example: Pass mark bugs often come from using > when the correct requirement is >=. <br>例子：及格线 bug 常常来自把 >= 写成了 >。 |

# 12\. How to use print debugging effectively / 怎样有效用 print 调试

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Print debugging print 调试** | print() is a simple but powerful beginner debug tool. <br>print() 是初学者非常简单但很强的调试工具。 | By printing variable values, branch choices, and loop progress, you make the invisible program state visible. <br>通过打印变量值、分支选择和循环进度，你可以把原本看不见的程序状态变成可见。 | Example: Print score, count, or current_max inside the loop to observe changes. <br>例子：在循环里打印 score、count 或 current_max 来观察变化。 |
| **Print before and after changes 改变前后都打印** | Printing both before and after a key update can show exactly where a value becomes wrong. <br>在关键更新前后都打印，可以精确看到值是从哪里开始变错的。 | This is especially useful in loops and conditional branches. <br>这在循环和条件分支里特别有用。 | Example: Print total before total += value and again after it. <br>例子：在 total += value 前打印一次 total，更新后再打印一次。 |
| **Print branch decisions 打印分支选择** | Printing which branch was taken helps you verify condition logic. <br>打印进入了哪个分支，可以帮助你验证条件逻辑。 | If the wrong branch runs, the bug is likely in the condition or in the values feeding it. <br>如果走错了分支，bug 很可能在条件本身，或者在喂给条件的值上。 | Example: Print "Entered pass branch" or "Entered fail branch" temporarily. <br>例子：临时打印 "Entered pass branch" 或 "Entered fail branch"。 |
| **Do not spam blindly 不要盲目乱 print** | Print debugging works best when targeted, not when every line prints everything. <br>print 调试最有效的时候，是有针对性，而不是每一行都乱打一堆。 | Too much output becomes noise and hides the important pattern. <br>输出太多会变成噪音，反而掩盖关键模式。 | Example: Print only the variables directly related to the bug, not every variable in the file. <br>例子：只打印和 bug 直接相关的变量，不要把文件里所有变量都打印。 |

# 13\. Complete Practical Example 1 / 完整实际例子 1

## Debugging a runtime error / 调试一个运行时错误

### Broken Code / 出错代码

age = int(input("Enter your age:"))  
print("Next year you will be", age + 1)

**Problem / 问题**

如果用户输入：

abc

程序会崩掉。

### Why it breaks / 为什么会崩

因为 int() 只能把合法数字文字转换成整数。  
"abc" 不是合法整数格式，所以会触发 ValueError。

### How to debug it / 怎样调试它

| **Step 步骤** | **English** | **中文** |
| --- | --- | --- |
| 1 | Reproduce the problem by entering abc. | 输入 abc，重现问题。 |
| 2 | Read the error type: ValueError. | 读错误类型：ValueError。 |
| 3 | Read the message: invalid text for integer conversion. | 读说明：文字无法转换成整数。 |
| 4 | Identify the critical line: int(input(...)). | 找关键行：int(input(...))。 |
| 5 | Realize the syntax is fine, but the value is invalid. | 明白语法没问题，问题在值不合法。 |
| 6 | Add input validation or error handling. | 加入输入验证或异常处理。 |

### Improved Version / 改进版

user_input = input("Enter your age: ")  
<br/>if user_input.isdigit():  
age = int(user_input)  
print("Next year you will be", age + 1)  
else:  
print("Please enter a valid number.")

# 14\. Complete Practical Example 2 / 完整实际例子 2

## Debugging a logic error / 调试一个逻辑错误

### Broken Code / 出错代码

score = 50  
<br/>if score > 50:  
print("Pass")  
else:  
print("Fail")

### Problem / 问题

题目要求：  
**50 and above = Pass**  
但这个程序把 50 判成 Fail。

### Why it breaks / 为什么会错

代码运行完全正常，没有崩。  
所以这不是 syntax error，也不是 runtime error。  
这是 **logic error**。

### How to debug it / 怎样调试它

| **Step 步骤** | **English** | **中文** |
| --- | --- | --- |
| 1 | Compare expected vs actual output. | 对比预期输出和实际输出。 |
| 2 | Expected: Pass for score 50. | 预期：50 分应该是 Pass。 |
| 3 | Actual: Fail. | 实际：却是 Fail。 |
| 4 | Inspect the condition carefully. | 仔细检查条件。 |
| 5 | Notice that > excludes 50. | 发现 > 会排除 50。 |
| 6 | Replace it with >=. | 把它改成 >=。 |

### Fixed Version / 修正版

score = 50  
<br/>if score >= 50:  
print("Pass")  
else:  
print("Fail")

# 15\. Complete Practical Example 3 / 完整实际例子 3

## Using print debugging / 用 print 调试

### Broken Code / 出错代码

numbers = \[10, 20, 30\]  
total = 0  
<br/>for number in numbers:  
total = number  
<br/>print("Total:", total)

### Problem / 问题

你可能想得到：

Total: 60

但实际输出是：

Total: 30

### Why it breaks / 为什么会错

因为在循环里你写的是：

total = number

这不是累加。  
这会让 total 每次都被当前 number 覆盖。  
最后只剩最后一个数 30。

### Use print to inspect / 用 print 检查

numbers = \[10, 20, 30\]  
total = 0  
<br/>for number in numbers:  
print("Before update:", total)  
print("Current number:", number)  
total = number  
print("After update:", total)  
<br/>print("Total:", total)

### What you will notice / 你会注意到什么

你会看到：

- total 不是一直增加
- 它每次直接变成当前的 number
- 所以最终只剩下 30

### Fixed Version / 修正版

numbers = \[10, 20, 30\]  
total = 0  
<br/>for number in numbers:  
total += number  
<br/>print("Total:", total)

# 16\. Debug Strategy Comparison Table / 调试策略对比表

| **Bad Debug Habit 坏调试习惯** | **Better Debug Habit 好调试习惯** |
| --- | --- |
| Panic when red text appears. <br>一看到红字就慌。 | Read the error type and message calmly. <br>冷静读错误类型和说明。 |
| Change many lines randomly. <br>随机改很多行。 | Change one thing at a time. <br>一次只改一个点。 |
| Ignore line numbers. <br>忽略行号。 | Use the line number as a starting clue. <br>把行号当作起点线索。 |
| Assume values without checking. <br>凭感觉猜变量值。 | Print or inspect actual values. <br>打印或检查真实变量值。 |
| Stop when code runs once. <br>只要跑过一次就停。 | Verify the fix with several test cases. <br>用多个测试案例验证修复。 |
| Treat bugs as proof of failure. <br>把 bug 当成失败证据。 | Treat bugs as information about what to learn next. <br>把 bug 当成下一步学习信息。 |

# 17\. Self-Check Table / 自我检查表

| **Question (English)** | **中文问题** |
| --- | --- |
| Can I explain the difference between syntax, runtime, and logic errors? | 我能解释语法错误、运行时错误、逻辑错误的区别吗？ |
| When my code crashes, do I first read the error type and line number? | 当代码崩掉时，我会先读错误类型和行号吗？ |
| Do I know how to use print to inspect variable values? | 我知道怎样用 print 检查变量值吗？ |
| When output is wrong, do I compare expected vs actual result? | 当输出不对时，我会比较预期结果和实际结果吗？ |
| Do I change one thing at a time, or do I randomly rewrite many lines? | 我是一次改一个点，还是会乱改很多行？ |
| After fixing a bug, do I test more than one case? | 修好一个 bug 后，我会测试不止一个案例吗？ |
| Can I stay calm enough to investigate instead of panicking? | 我能不能保持冷静去调查，而不是先慌？ |

# 18\. Key Takeaways / 本课核心重点

| **Type 类型** | **Core Idea 核心概念** | **How it works 它如何运作** | **Usage / Example 用途 / 例子** |
| --- | --- | --- | --- |
| **Debugging is investigation 调试是一种调查** | Debugging means finding why code behavior differs from expectation. <br>调试就是找出代码行为为什么和预期不一样。 | You inspect clues instead of guessing wildly. <br>你要检查线索，而不是乱猜。 | Example: error type, line number, variable value, wrong branch choice. <br>例子：错误类型、行号、变量值、进入了错误分支。 |
| **There are different bug types bug 有不同类型** | Syntax, runtime, and logic errors need slightly different debug approaches. <br>语法错误、运行时错误、逻辑错误需要略有不同的调试方式。 | Knowing the type gives you the right starting direction. <br>知道类型，就会知道该从哪里开始。 | Example: syntax → structure; runtime → actual values; logic → expected vs actual behavior. <br>例子：语法 → 结构；运行时 → 真实值；逻辑 → 预期与实际行为。 |
| **Print is a beginner superpower print 是初学者超强工具** | print() can reveal invisible state and execution flow. <br>print() 可以让看不见的状态和执行流程变得可见。 | You inspect variables, branches, and loop progress directly. <br>你可以直接检查变量、分支和循环进度。 | Example: print values before and after updates. <br>例子：在更新前后都打印值。 |
| **One change at a time 一次只改一个点** | Random large edits make debugging worse. <br>大范围乱改会让调试更糟。 | Small controlled changes reveal what actually fixed the issue. <br>小而可控的修改，才能看出到底是什么修好了问题。 | Example: fix condition first, then retest, then inspect next issue if needed. <br>例子：先改条件，再测试，再决定是否继续查别的问题。 |
| **Bugs are part of learning bug 是学习的一部分** | Every bug teaches you something about syntax, logic, values, or flow. <br>每个 bug 都会教你一些关于语法、逻辑、值或流程的东西。 | Fixing bugs strengthens future pattern recognition. <br>修 bug 会强化你未来的模式识别能力。 | Example: after many type conversion bugs, you naturally become more careful with input handling. <br>例子：修多了类型转换错误后，你会自然更小心处理输入。 |
