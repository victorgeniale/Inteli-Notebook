# Refatoração
- Adição de novas funcionalidades requerem uma nova refatoração;
- Correção de bugs requerem uma nova refatoração;
- Revisões de código requerem uma nova refatoração;

## Métodos de refatoração
- Pull-up field/method: Quando há 2 subclasses com o mesmo atributo/método, esse atributo/método é movido para a super classe para evitar duplicados;
<p align="center">
  <img width=50% src="https://i.imgur.com/0psrT8k.gif">
</p>
- Pull-down field/method: Quando comportamento é relevante somente para uma subclasse, o atributo/método é movido para ela;
- Extract subclass: Quando uma classe for apenas utilizável em algumas instâncias, mover as funcionalizades dessa classe para outra mais especializada;
- Extract superclass: Quando duas classe possuem características em comum, mover as funcionalizades dessa classe para outra superclasse mais especializada;
- Replace temp with query: Substitui variáveis temporárias por método que retorne o valor dessa expressão;

# DEBUG
## Uso de print()
> Ao usar prints dentro de uma fração do código, pode ser checado a sua usabilidade e possíveis erros contídos nele;
```Python
varA = 1
varB = 2

def foo():
	...

while varA > varB:
	print("A>B")  # DEBUG
	foo()
else:  # DEBUG
	print("Code is wrong.")
```
.>>> Code is wrong.
- A mensagem "code is wrong." demonstra que a tarefa **while** nunca é executada, algo identificado pelo print(). Se o **while** fosse executado, a mensagem "A>B" tornaria isso claro para o dev.
# Os 3 aspectos para provar a qualidade do software
1. Qualidade funcional: O software performa as tarefas necessárias, tem boa performance e são acessíveis para um usuário qualquer;
2. Qualidade estrutural: O software está organizado em uma maneira que o torna fácil de ser testado, incrementado e entendido, ele também deve promover uma boa segurança;
3. Qualidade processual: O software não pode ser contruido de uma maneira em que os prazos estabelescidos sejam violados, bem como ir além do orçamento e sobrecarregar os desenvolvedores;