# Posicionamento

O posicionamento no CSS é uma técnica que permite controlar como os elementos são dispostos na página. Ele é fundamental para a criação de layouts responsivos e bem estruturados, garantindo que os elementos apareçam corretamente em diferentes dispositivos e resoluções de tela.

A escolha correta do tipo de posicionamento é essencial para garantir a manutenibilidade e o desempenho da aplicação web, evitando sobreposições indesejadas e problemas de usabilidade.

### static

Posicionamento padrão de todos os elementos HTML. Os elementos são posicionados de acordo com o fluxo normal do documento, trazendo simplicidade e previsibilidade, porém tem a desvantagem de não ter a flexibilidade para sobrepor ou ajustar posições. É utilizado por padrão e pode ser utilizado sempre que não houver a necessidade de algum tipo de posicionamento especial.

#### Exemplo

```css
p {
  position: static;
}
```
---
### relative

O elemento é posicionado com relação à sua posição original, mantendo o espaço original ocupado e com flexibilidade para pequenos deslocamentos, porém não sai do fluxo do documento. Utilizado para fazer pequenos ajustes sem afetar os outros elementos.

#### Exemplo

```css
div {
  position: relative;
  top: 20px;
  left: 10px;
}
```
---
### absolute

Remove o elemento do fluxo do documento e o posiciona em relação ao elemento ancestral com `position: relative`, ou ao body caso não haja nenhum ancestral posicionado. Possui algumas vantagens como precisão total no posicionamento e também não afeta outros elementos, porém pode causar sobreposição inesperadas e não é responsivo por padrão. Utilizado quando é necessário posicionamento preciso em relação a outro elemento.

#### Exemplo

```css
div {
  position: absolute;
  top: 50px;
  right: 30px;
}
```
---
### fixed

O elemento é posicionado em relação à janela de visualização (viewport), permanecendo fixo mesmo ao rolar a página, sempre visível ao usuário, porém pode sobrepor outros elementos. Utilizado por exemplo para elementos como menus fixos e botões de volta ao topo.

#### Exemplo

```css
div {
  position: fixed;
  bottom: 10px;
  right: 10px;
}
```
---
### float

Permite que elementos "flutuem" para o lado esquerdo ou direito, permitindo que outros elementos fluam ao seu redor, tem boa compatibilidade com navegadores mais antigos, porém é difícil de controlar espaçamentos e pode causar problemas de colapsos com contêineres. Era utilizado para construir layouts antes do flexbox e do grid.

#### Exemplo

```css
div {
  float: left;
  width: 50%;
}
```
---
### z-index

Controla a ordem de empilhamento (eixo z) dos elementos na página, elementos com valor `z-index` maior aparecem na frente de elementos com valor menor. Sua vantagem é o controle preciso sobre a hierarquia visual, porém pode criar confusão se não usado corretamente. Utilizado para garantir a sobreposição correta de elementos.

#### Exemplo

```css
div {
  position: absolute;
  z-index: 10;
}
```
---
### display

Define como um elemento é exibido na página, técnica mais utilizada nos dias atuais para trabalhar com layouts responsivos utilizando flexbox e grid layout. 

Valores comuns:

- `block`: Ocupa toda a largura disponível.
- `inline`: Ocupa apenas o espaço necessário.
- `inline-block`: Comporta-se como `inline`, mas respeita espaçamentos.
- `flex`: Permite layouts flexíveis.
- `grid`: Usa um sistema de grade.

#### Exemplo:

```css
div {
  display: flex;
  justify-content: center;
}
```
---
[Aula prática](https://www.notion.so/Aula-pr-tica-24fd15a33297816b9048c4fc03ad1fd9?pvs=21)

## Referências

[Entenda de uma vez por toda position ABSOLUTE e RELATIVE | ilustraCode](https://www.youtube.com/watch?v=5elYAmzXQ6M&ab_channel=ilustraCode-Programa%C3%A7%C3%A3oWeb)

[Entenda o position ABSOLUTE, RELATIVE, FIXED e Z-INDEX](https://www.youtube.com/watch?v=7svFaPgLCnc&ab_channel=ThiagoFranchin)

[[CSS5 - tópico 4] Posicionamento fixo em CSS (position: fixed)](https://www.youtube.com/watch?v=1UgayEekzHk&ab_channel=Fl%C3%A1vioCoutinho)

[Curso de HTML e CSS - Z-index [Aula 24]](https://www.youtube.com/watch?v=VP1Aw-qMMnI&ab_channel=ChiefofDesign)

[Para que serve e como usar o FLOAT CSS | ilustraCode](https://www.youtube.com/watch?v=BHSfMqefFss&ab_channel=ilustraCode-Programa%C3%A7%C3%A3oWeb)

[Curso de HTML e CSS - Float Left, Right [Aula 25]](https://www.youtube.com/watch?v=Ef4UZffzKEA&pp=ygUYcG9zaWNpb25hbWVudG8gY3NzIGZsb2F0)

[Aprenda CSS Position em 10 Minutos - Tutorial CSS para Iniciantes](https://www.youtube.com/watch?v=zPlt84S1L0U&ab_channel=TigerCodes)

[OS TIPOS DE DISPLAY DOS ELEMENTOS - HTML E CSS](https://www.youtube.com/watch?v=XTnr1DpHfKo&ab_channel=EduardoMota)
