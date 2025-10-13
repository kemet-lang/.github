<!----------------------------------- BEG ----------------------------------->
<br>
<div align="center">
    <p>
        <img src="../assets/img/logo.png" alt="Kemet-Logo" style="" width="300" />
    </p>
</div>


<div align="center">
    <p>
        <img src="../assets/img/lang-desc.png" alt="Kemet-Desc" style="" width="220" />
    </p>
    <img src="https://img.shields.io/badge/v-MVP-black"/>
    <a href="../README.md"><img src="https://img.shields.io/badge/from-kemet_lang-black"/></a>
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

    > Actually.. **What am I trying to do here?** How will Kemet ultimately work? **What is the nature of the program I'm trying to build here?** well, this question is not easy, so **[What is my goal?](#target)** and **[How will I achieve it?](#workflow)**

<br>
<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block;width:500px;"/>
    <br>
</div>

- ### Target

    > A **vscode extention** including **syntax highlighter** and **[language server](#kemet-language-server)**.

    - #### Kemet Language Server

        > I have tried dozens of languages in my life. There are great languages, but their LSP is sterile/barren, and there are languages that are not of the same quality, but they have a superb LSP that makes the development process much better, like TypeScript's.

        > And in fact, I don't intend to build something sterile/inadequate, or at least I don't want to wait long before enjoying writing code in the Kemet language with at least the same quality that I enjoy when writing TypeScript.

        > As you can see, I thought first about the LSP. Anyone in my place would have thought about other things like the language syntax! Simply put, the hard part is not building a programming language, **But building an experience that makes programming without Kemet a waste of time!**

        - ##### Why vscode? is it enough?

            > temp solution, yes it's enough for now.

        - ##### Which language will use?

            > vscode uses **TypeScript** so i will use it too.

        > The **[main repo](https://github.com/kemet-lang/core)** will contain the vscode extension as a wrapper for our [@je-es/lsp](https://github.com/je-es/lsp) and [@je-es/project](https://github.com/je-es/project) libraries.

        > By using my [`je-es`](https://github.com/je-es) framework, I'm reducing direct friction with vscode and working on small, separate libraries that are easier to maintain and reuse again if we want to, without rewriting or duplicating the same logic and code again.

        > Honestly, this approach is the best. You can imagine it as if I've turned what I'm doing into a pharaonic puzzle - to solve it, you must gather and assemble all the pieces together correctly, which is what I will do and explain next.

        > In other words, I will create a set of well-polished pieces individually, each piece separately, and I will only assemble them together at the end and put the configuration I want in a way that aligns with Kemet's principles. This means that everything I'm building now **can be reused to build any other language and not just Kemet!**

<br>
<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block;width:500px;"/>
    <br>
</div>

- ### Workflow

    | target                                                   | desc                                                          | namespace    | status           |
    | -------------------------------------------------------- | ------------------------------------------------------------- | ------------ | ---------------- |
    | `01` [`lexer`](https://github.com/je-es/lexer)           | A tool for converting text into tokens.                       | `je-es`      | `100%` `live`    |
    | `02` [`parser`](https://github.com/je-es/parser)         | A mechanism for creating grammatical rules.                   | `je-es`      | `100%` `live`    |
    | `03` [`syntax`](https://github.com/je-es/syntax)         | A wrapper for lexer and parser.                               | `je-es`      | `100%` `live`    |
    | `04` [`ast`](https://github.com/je-es/ast)               | A library for building and managing Abstract Syntax Trees.    | `je-es`      | `-99%` `local`   |
    | `05` [`rules`](https://github.com/kemet-lang/rules)      | Shared kemet language rules.                                  | `kemet-lang` | `-99%` `local`   |
    | `06` [`analyzer`](https://github.com/je-es/ast-analyzer) | A library for analyzing and validating Abstract Syntax Trees. | `je-es`      | `-99%` `local`   |
    | `07` [`project`](https://github.com/je-es/project)       | ...                                                           | `je-es`      | `-60%` `local`   |
    | `08` [`lsp`](https://github.com/je-es/lsp)               | ...                                                           | `je-es`      | `-50%` `local`   |
    | `09` [`core`](https://github.com/kemet-lang/core)        | main repo.                                                    | `kemet-lang` | `--0%` `local`   |
    | `10` [`codegen`](https://github.com/je-es/codegen)       | ...                                                           | `je-es`      | `--0%` `not-yet` |
    | `11` [`compiler`](https://github.com/je-es/compiler)     | ...                                                           | `je-es`      | `--0%` `not-yet` |


<br>
<div align="center">
    <img src="../assets/img/line.png" alt="line" style="display: block;width:500px;"/>
    <br>
</div>

<!--------------------------------------------------------------------------->



<!----------------------------------- END ----------------------------------->

<br>
<div align="center" dir='rtl'>
    <a href="https://github.com/maysara-elshewehy">
        <img src="https://img.shields.io/badge/by-Maysara-blue"/>
    </a>
</div>

<!--------------------------------------------------------------------------->
