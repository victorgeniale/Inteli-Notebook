# Variávies
- **Não** podem começar com números ou conter espaços e sinais de operação;
- **Não** podem contem letras maiúsculas e minúsculas como única diferença

# Cool Hax
- Formatação de uma string pode ser feita assim:
```Python
varA = "Scott"
varB = "Coffee"
print(f"These are my favorite things: {varA} & {varB}")
```
.>>> These are my favorite things: Scott & Coffee

- Pode-se usar match case para substituir vários elifs:
```Python
command = "Hello, World!"
match command:
	case "Hello, World!":
		print("Hello there")
	case "Goodbye, World!":
		print("Bye Then...")
	case other:
		print("No match found, Try again!")
```
.>>> Hello there