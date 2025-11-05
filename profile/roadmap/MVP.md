<!----------------------------------- BEG ----------------------------------->
<br>
<div align="center">
    <p>
        <img src="../assets/img/logo.png" alt="Kemet-Logo" style="" width="300" />
    </p>
</div>


<div align="center">
    <p>
        <img src="../assets/img/mvp-desc.png" alt="Kemet-Desc" style="" width="300" />
    </p>
    <img src="https://img.shields.io/badge/Version-MVP-black"/>
    <a href="../README.md"><img src="https://img.shields.io/badge/Built_for-kemet_lang-black"/></a>
</div>


<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block; margin-top:20px;margin-bottom:20px;width:500px;"/>
    <br>
</div>

<!--------------------------------------------------------------------------->



<!----------------------------------- --- ----------------------------------->

- ### Minimum Viable Product (MVP)

    > As I write these lines, **there is no Kemet yet**, so naturally I'll **use another programming language** to **build the first version of Kemet**, and then I'll use that version to build another version — **But this time using Kemet itself!**

    > In Kemet, I'm not trying to build something that just works! There are plenty of things that already work! What I'm trying to do here is **build a civilization** — **My Civilization**.

    > Most people start by building a poorly-designed program in a matter of days, call it their first release, and then spend years fixing issues that could have been avoided from **the beginning—technical debt**.

    > Actually.. **What am I trying to do here?** How will Kemet ultimately work? **What is the nature of the program I'm trying to build here?** well, this question is not easy, so **[What is my goal?](#kemet-lang)** and **[How will I achieve it?](#workflow)**

<br>
<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block;width:500px;"/>
    <br>
</div>

- ### Workflow

    ![img](../assets/img/diag.svg)

    - #### `@je-es`

        > By using my [`je-es`](https://github.com/je-es) framework, I'm reducing direct friction with vscode and working on small, separate libraries that are easier to maintain and reuse again if we want to, without rewriting or duplicating the same logic and code again.

        > In other words, I will create a set of well-polished pieces individually, each piece separately, and I will only assemble them together at the end and put the configuration I want in a way that aligns with Kemet's principles. This means that everything I'm building now **can be reused to build any other language and not just Kemet!**


        | target                                                              | desc                                                    | status |
        | ------------------------------------------------------------------- | ------------------------------------------------------- | ------ |
        | `01` [`@je-es/lexer`](https://github.com/je-es/lexer)               | Converts source code into token streams for parsing.    | `dev`  |
        | `02` [`@je-es/parser`](https://github.com/je-es/parser)             | Builds Abstract Syntax Trees from token streams.        | `dev`  |
        | `03` [`@je-es/ast`](https://github.com/je-es/ast)                   | Defines AST structure for analysis and code generation. | `dev`  |
        | `04` [`@je-es/syntax`](https://github.com/je-es/syntax)             | Defines formal grammar and syntax rules.                | `dev`  |
        | `05` [`@je-es/ast-analyzer`](https://github.com/je-es/ast-analyzer) | Performs static analysis and semantic validation.       | `dev`  |
        | `06` [`@je-es/codegen`](https://github.com/je-es/codegen)           | Generates target code from AST.                         | `50%`  |
        | `07` [`@je-es/project`](https://github.com/je-es/project)           | Manages single projects for CLI/LSP integration.        | `dev`  |
        | `08` [`@je-es/lsp`](https://github.com/je-es/lsp)                   | Language server with full VSCode integration.           | `dev`  |
        | `09` [`@je-es/compiler`](https://github.com/je-es/compiler)         | Complete compilation pipeline orchestrator.             | `0%`   |

    - #### `@kemet-lang`

        | target                                                        | desc                                                      | status |
        | ------------------------------------------------------------- | --------------------------------------------------------- | ------ |
        | `01` [`@kemet-lang/sesh`](https://github.com/kemet-lang/sesh) | Grammar rules, syntax definitions, and LSP configuration. | `99%`  |
        | `02` [`@kemet-lang/core`](https://github.com/kemet-lang/core) | Core language implementation and runtime.                 | `99%`  |
        | `03` [`@kemet-lang/cli`](https://github.com/kemet-lang/cli)   | Command-line interface for Kemet projects.                | `99%`  |
        | `04` [`@kemet-lang/vsc`](https://github.com/kemet-lang/vsc)   | VSCode extension for Kemet language support.              | `99%`  |
        | `05` [`@kemet-lang/web`](https://github.com/kemet-lang/web)   | Web-based Kemet playground and documentation.             | `99%`  |


<br>
<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block;width:500px;"/>
    <br>
</div>

<!--------------------------------------------------------------------------->



<!----------------------------------- END ----------------------------------->

<br>
<div align="center" dir='ltr'>
    <a href="https://github.com/maysara-elshewehy">
        <img src="https://img.shields.io/badge/by-Maysara-blue"/>
    </a>
</div>
<div align="center" dir='ltr'>
    <img src="https://img.shields.io/badge/-5 dec 2025-black"/>
</div>

<!--------------------------------------------------------------------------->