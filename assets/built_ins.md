# 🐍 Python Built-in Functions Cheat Sheet

---

## 🟢 **Type Conversion**

| Function | Description | Example |
|----------|-------------|---------|
| `int()` | Convert to integer | `int("42")` → `42` |
| `float()` | Convert to float | `float("3.14")` → `3.14` |
| `str()` | Convert to string | `str(123)` → `"123"` |
| `bool()` | Convert to boolean | `bool(0)` → `False` |
| `complex()` | Create complex number | `complex(1, 2)` → `(1+2j)` |
| `list()` | Convert to list | `list("abc")` → `['a', 'b', 'c']` |
| `tuple()` | Convert to tuple | `tuple([1, 2])` → `(1, 2)` |
| `set()` | Convert to set | `set([1, 2, 2])` → `{1, 2}` |
| `dict()` | Create dictionary | `dict(a=1, b=2)` → `{'a': 1, 'b': 2}` |
| `frozenset()` | Immutable set | `frozenset([1, 2])` |
| `bytes()` | Convert to bytes | `bytes("abc", "utf-8")` |
| `bytearray()` | Mutable byte array | `bytearray("abc", "utf-8")` |
| `memoryview()` | View of memory buffer | `memoryview(b"abc")` |

---

## 🔁 **Iterables & Functional Tools**

| Function | Description | Example |
|----------|-------------|---------|
| `len()` | Length of object | `len("abc")` → `3` |
| `range()` | Range of numbers | `range(5)` → `0..4` |
| `enumerate()` | Index + value | `enumerate(["a", "b"])` |
| `zip()` | Combine iterables | `zip([1,2], [3,4])` |
| `map()` | Apply function | `map(str, [1, 2])` |
| `filter()` | Filter items | `filter(bool, [0, 1])` |
| `reversed()` | Reverse iterator | `reversed([1, 2, 3])` |
| `sorted()` | Return sorted list | `sorted([3, 1, 2])` |
| `all()` | All true? | `all([True, True])` |
| `any()` | Any true? | `any([False, True])` |
| `sum()` | Sum values | `sum([1, 2, 3])` |

---

## 🔣 **Input / Output**

| Function | Description | Example |
|----------|-------------|---------|
| `print()` | Print to stdout | `print("Hello")` |
| `input()` | Get user input | `name = input()` |
| `format()` | Format string | `"{}".format(42)` |
| `ascii()` | Printable ASCII | `ascii("€")` → `'\\u20ac'` |
| `repr()` | Printable object | `repr("hi")` → `'hi'` |
| `chr()` | Int → Unicode char | `chr(65)` → `'A'` |
| `ord()` | Unicode char → Int | `ord("A")` → `65` |
| `bin()` | Int → Binary str | `bin(10)` → `'0b1010'` |
| `oct()` | Int → Octal str | `oct(8)` → `'0o10'` |
| `hex()` | Int → Hex str | `hex(255)` → `'0xff'` |

---

## 🧠 **Object & Introspection**

| Function | Description | Example |
|----------|-------------|---------|
| `type()` | Type of object | `type(3)` → `<class 'int'>` |
| `isinstance()` | Check type | `isinstance(3, int)` |
| `id()` | Object identity | `id(obj)` |
| `dir()` | Attributes & methods | `dir(str)` |
| `vars()` | `__dict__` of obj | `vars(obj)` |
| `callable()` | Is callable? | `callable(len)` |
| `hasattr()` | Has attribute? | `hasattr(obj, 'x')` |
| `getattr()` | Get attr | `getattr(obj, 'x')` |
| `setattr()` | Set attr | `setattr(obj, 'x', 42)` |
| `delattr()` | Delete attr | `delattr(obj, 'x')` |

---

## 🔒 **Evaluation & Compilation**

| Function | Description | Example |
|----------|-------------|---------|
| `eval()` | Eval string | `eval("2 + 2")` → `4` |
| `exec()` | Execute code | `exec("x = 3")` |
| `compile()` | Compile code object | `compile("x=1", "", "exec")` |

---

## 📚 **Help & Utilities**

| Function | Description | Example |
|----------|-------------|---------|
| `help()` | Interactive help | `help(str)` |
| `globals()` | Global symbol table | `globals()` |
| `locals()` | Local symbol table | `locals()` |
| `__import__()` | Dynamic import | `__import__('math')` |

---

## 🔢 **Mathematics & Numbers**

| Function | Description | Example |
|----------|-------------|---------|
| `abs()` | Absolute value | `abs(-5)` → `5` |
| `pow()` | Exponentiation | `pow(2, 3)` → `8` |
| `round()` | Round value | `round(3.1415, 2)` |
| `divmod()` | Division + remainder | `divmod(9, 4)` → `(2, 1)` |
| `max()` | Maximum value | `max(1, 2, 3)` |
| `min()` | Minimum value | `min([1, 2])` |

---

## 🔧 **Classes, Inheritance, Objects**

| Function | Description | Example |
|----------|-------------|---------|
| `object()` | Base class | `o = object()` |
| `classmethod()` | Define class method | `@classmethod` |
| `staticmethod()` | Define static method | `@staticmethod` |
| `property()` | Create property | `@property` |
| `super()` | Call superclass | `super().__init__()` |

---

## ⚠️ **Exception Handling**

| Function | Description | Example |
|----------|-------------|---------|
| `abs()` | Absolute value | `abs(-7)` → `7` |
| `all()` | Are all true? | `all([True, True])` |
| `any()` | Is any true? | `any([False, True])` |
| `breakpoint()` | Start debugger | `breakpoint()` |
| `BaseException`, `Exception`, etc. | Exception base classes | `raise Exception("Oops!")` |

---

## 🗑️ **Other Utilities**

| Function | Description | Example |
|----------|-------------|---------|
| `open()` | Open file | `open("file.txt")` |
| `del` | Delete variable | `del x` |
| `pass` | Do nothing | `pass` |
| `ellipsis` | `...` for slicing | `a[...]` |

---

## 📜 Get Full List in Code

```python
import builtins
print(dir(builtins))
```
