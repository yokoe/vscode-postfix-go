# Postfix templates for Golang
[![Version](https://vsmarketplacebadge.apphb.com/version-short/yokoe.vscode-postfix-go.svg
)](https://marketplace.visualstudio.com/items?itemName=yokoe.vscode-postfix-go)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/yokoe.vscode-postfix-go.svg
)](https://marketplace.visualstudio.com/items?itemName=yokoe.vscode-postfix-go)

Forked from [vscode-postfix-ts](https://github.com/ipatalas/vscode-postfix-ts)

Under development. Any suggestions are welcomed.

## Templates

All available templates (`expr` means the expression on which the template is applied):

| Template          | Outcome |
| -------:          | ------- |
| **.if**           | `if expr` |
| **.else**         | `if !expr` |
| **.nil**         | `if expr == nil` |
| **.notnil**      | `if expr != nil` |
| **.nilr**      | `if expr == nil  { return expr }` |
| **.must**      | `if expr != nil  { return expr }` |
| **.for**          | `for index, element := range expr` |
| **.return**       | `return expr` |
| **.var**          | `name := expr` |
| **.const**          | `const name type = expr` |
| **.append**          | `expr = append(expr, element)` |
| **.print**          | `fmt.Println(expr)` |
| **.printf**          | `fmt.Printf("%+v\n", expr)` |
| **"expr".error**          | `errors.New("expr")` |

## Author

Sota Yokoe [@croquette0212](https://twitter.com/croquette0212)

## Contributors
[Hamza Anis](https://github.com/HamzaAnis)