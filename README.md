
## 🔤 Custom Programming Language (Hindi-Inspired)

**A Python-based interpreter for a Hindi-style programming language** supporting variables, arithmetic, conditionals, loops, and functions with an interactive REPL and helpful error handling.

> Educational project to explore language design and compiler/interpreter construction.


## 🌟 Features

* ✅ **Hindi-Inspired Syntax**

  * `VAR`, `AGAR`, `WARNA`, `JABTAK`, `KE_LIYE`, `FUNK`, etc.
* ✅ **Core Language Features**

  * Variables: `VAR x = 5 + 3`
  * Arithmetic: `+`, `-`, `*`, `/`, `**`
  * Conditionals: `AGAR x < 5 TAB 0 WARNA x`
  * Loops: `KE_LIYE i = 1 TAK 3 KADAM 1 TAB i`
  * Functions: `FUNK multi(x, y) -> x * y`
* ✅ **Interactive REPL Interface** (`shell.py`)
* ✅ **Descriptive Error Handling** with source highlighting (`strings_with_arrows.py`)
* ✅ **Grammar-Driven Design** via `grammar.txt` (easily extensible)

---

## 🗂️ Project Structure

```
custom_programming_language/
├── basic.py                # Lexer, Parser, Interpreter logic
├── shell.py                # REPL interface
├── strings_with_arrows.py # Error formatting utilities
├── grammar.txt             # Grammar definition
└── README.md               # Documentation
```

---

## ⚙️ Setup

### 🔧 Prerequisites

* Python 3.8 or above
* No external libraries needed (uses Python Standard Library)

### 📥 Installation

```bash
git clone https://github.com/Arihant0908/custom_programming_language.git
cd custom_programming_language
python --version  # Make sure Python 3.8+ is installed
```

---

## 💡 Usage

### ▶️ Start the REPL:

```bash
python shell.py
```

### 📌 Example REPL Commands:

```txt
basic > VAR x = 5 + 3
8

basic > AGAR x < 10 TAB 1 WARNA 0
1

basic > KE_LIYE i = 1 TAK 3 KADAM 1 TAB i
[1, 2, 3]

basic > FUNK multi(x,y) -> x*y
<function multi>

basic > multi(2,3)
6
```

Use `Ctrl+C` to exit the REPL.

---

## 📚 Language Grammar

Defined in `grammar.txt`. Examples:

* **Variable Declaration**:
  `VAR x = 5 + 3`

* **Conditionals**:
  `AGAR x < 10 TAB 1 WARNA 0`

* **For Loop**:
  `KE_LIYE i = 1 TAK 3 KADAM 1 TAB i`

* **While Loop**:
  `JABTAK x < 5 TAB x + 1`

* **Function**:
  `FUNK add(a,b) -> a + b`

---

## ✅ Testing & Validation

* Lexer: Tokenization of input like `VAR x = 5 + 3`
* Parser: Builds AST for expressions, loops, conditionals
* Interpreter: Successfully evaluates complex expressions and control flow
* REPL tested for interaction and error catching

---

## 🧠 Challenges Overcome

* 🛠️ Operator precedence handled using custom `bin_op` logic
* 🧪 Fixed token mismatches in nested structures using parser lookahead
* 📛 Improved user feedback with custom error pointers (`strings_with_arrows.py`)

---

## 🔮 Future Scope

* 🚀 Host the REPL online (e.g., with Vercel or Replit)
* 🧩 Add more built-in functions and types
* ➕ Extend grammar to support `break`, `continue`, and `return` statements

