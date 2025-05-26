# rust-study


## 词法结构


Rust编译过程

rust是编译型语言，它的编译器叫做rustc， rustc是多道编译器， 编译过程需要经过多道工序

Rust Code （UTF-8）输入到编译器 -> 经过分词，把词法结构处理为词条流 -> 词条流经过语法解析生成AST抽象语法树 -> 将AST降级形成高级中间语言HIR (高级中间语言用于编译器对代码类型检查， 方法查找等工作) -> 进一步降级，形成中级中间语言MIR（中级中间语言用于借用检查， 优化， 代码生成 -> 优化生成LLVM中间语言，交由LLVM后端去生成机器码 -> 最后生成机器码

<img width="1409" alt="image" src="https://github.com/user-attachments/assets/3031da8e-12fe-470d-8670-0ac338404474" />


六大词法结构：

