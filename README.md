# 🧮 Regular Expression Generator for Σ = {a, b}

This is a web-based application developed as a part of the **Theory of Automata** course. It takes natural language descriptions of simple regular languages over the binary alphabet **Σ = {a, b}** and returns the corresponding **regular expression**.

## 🌐 Live Demo

Open the `indx.html` file in any modern web browser to run the application locally.

## 📌 Objective

To create an interactive interface that:
- Accepts basic language descriptions from users.
- Parses key patterns in the description.
- Generates a matching **regular expression**.

This project helps demonstrate the practical interpretation of automata theory and regular languages.

## 🧠 Supported Descriptions

The generator currently recognizes the following patterns:

| Description Example                            | Output Regular Expression      |
|------------------------------------------------|--------------------------------|
| begins with a                                  | `a(a|b)*`                      |
| ends with a                                    | `(a|b)*a`                      |
| ends with b                                    | `(a|b)*b`                      |
| contains ab                                    | `(a|b)*ab(a|b)*`               |
| begin with a and end with a                    | `a(a|b)*a`                     |
| begin with a and end with b                    | `a(a|b)*b`                     |
| begin with letter and end with same            | `(a(a|b)*a)|(b(a|b)*b)`        |
| only a                                         | `a*`                           |
| only b                                         | `b*`                           |
| no consecutive b                               | `(a|ba)*`                      |
| even number of a                               | `((b*ab*a)*b*)*`               |
| exactly two a                                  | `b*ab*ab*`                     |

_Note: Descriptions must closely match the phrases above to work correctly._

## 🧾 How to Use

1. **Open** the `indx.html` file in a web browser.
2. **Type** a language description like `"begins with a"` or `"contains ab"` in the text area.
3. **Click** the **"Generate Regex"** button.
4. View the resulting **regular expression** shown on the screen.

## 📁 Project Structure

