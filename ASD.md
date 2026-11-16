# Aplicação do ASD no projeto EntregaJá

## 1. Contexto

O EntregaJá é um protótipo acadêmico de um aplicativo de delivery de comida,
desenvolvido para a disciplina de Engenharia de Software. O objetivo foi criar
uma experiência simples para o usuário escolher um restaurante, consultar o
cardápio, selecionar produtos e finalizar um pedido.

O projeto foi conduzido usando o **ASD — Adaptive Software Development**
(Desenvolvimento Adaptativo de Software), uma metodologia ágil que aceita
mudanças durante o desenvolvimento e utiliza ciclos de especulação,
colaboração e aprendizado.

## 2. O que é ASD

O ASD foi criado por Jim Highsmith e Sam Bayer e é inspirado na ideia de que
projetos de software são sistemas complexos, sujeitos a mudanças e descobertas.
Por isso, em vez de tentar definir tudo antecipadamente, a equipe trabalha com
uma missão clara, ciclos curtos, protótipos e feedback contínuo.

As três fases do ciclo de vida são:

1. **Especulação:** define a missão, os objetivos, as restrições, o prazo e as
   hipóteses iniciais do projeto.
2. **Colaboração:** a equipe trabalha em conjunto, troca informações, toma
   decisões e constrói uma versão funcional do produto.
3. **Aprendizado:** a solução é testada, revisada e melhorada com base no
   resultado observado e no feedback recebido.

O ciclo é iterativo: depois do aprendizado, novas decisões podem levar a outra
   rodada de especulação, colaboração e aprendizado.

## 3. Aplicação no EntregaJá

### 3.1 Especulação

No início, não havia uma decisão final sobre o visual da tela. A missão foi
definida como:

> Criar uma tela mobile-first de delivery que permita escolher um restaurante,
> montar um pedido e simular sua finalização em um navegador, sem servidor.

As restrições e hipóteses iniciais foram:

- criar tudo em um único arquivo HTML;
- usar apenas HTML, CSS e JavaScript;
- não utilizar bibliotecas externas;
- trabalhar com dados fictícios;
- entregar um protótipo funcional em aproximadamente 20 minutos;
- começar pelo layout de celular e adaptar para telas maiores;
- deixar pagamentos reais, banco de dados e autenticação fora do escopo.

Como o design ainda não estava definido, foram propostas três alternativas:

1. **Lista moderna:** restaurantes apresentados em cards completos;
2. **Categorias:** descoberta por tipos de comida;
3. **Destaque visual:** restaurante recomendado em evidência, categorias e
   restaurantes próximos.

### 3.2 Colaboração

As alternativas foram apresentadas para decisão. A opção escolhida foi a
**ideia 3 — Destaque visual**. A partir dela, o fluxo foi refinado para:

1. escolher o restaurante;
2. abrir o cardápio;
3. escolher os produtos;
4. ir para o checkout e finalizar o pedido.

Esse fluxo foi implementado em uma página única, com navegação entre telas,
cards de restaurantes, categorias, cardápio, carrinho, formulário de checkout e
tela de confirmação.

### 3.3 Aprendizado

Após a implementação, o protótipo foi aberto e validado no navegador. O ciclo
permitiu confirmar que:

- a tela inicial funciona melhor com um restaurante recomendado em destaque;
- os botões precisam ser grandes para facilitar o uso em dispositivos móveis;
- o carrinho fixo facilita a passagem do cardápio para o checkout;
- o checkout pode ser demonstrado sem integrar um pagamento real;
- o projeto pode ser publicado no GitHub Pages sem servidor próprio.

O resultado foi ajustado e publicado em:

<https://karlouchoa.github.io/meucardapio/>

## 4. Artefatos produzidos

- **Protótipo visual:** três alternativas de design para a tela inicial;
- **Decisão de design:** escolha da alternativa 3;
- **Implementação:** `index.html`, contendo HTML, CSS e JavaScript;
- **Documentação:** `README.md` e este arquivo `ASD.md`;
- **Demonstração:** aplicação publicada no GitHub Pages.

## 5. Benefícios e limitações observados

O ASD foi útil porque permitiu começar mesmo sem uma decisão visual completa.
A criação de alternativas reduziu a incerteza e a escolha feita durante o
processo direcionou a implementação.

Como limitação, o protótipo não representa um sistema de produção: não possui
backend, banco de dados, autenticação, pagamento real ou acompanhamento de
entrega. Essas funcionalidades ficaram fora do escopo para preservar o prazo
e o objetivo acadêmico da atividade.

## 6. Referências

- [TreinaWeb — O que é ASD](https://www.treinaweb.com.br/blog/o-que-e-asd-adaptative-software-development)
- [Abstracta — Desenvolvimento Adaptativo de Software](https://abstracta.us/pt/blog/desenvolvimento/desenvolvimento-software-adaptativo-asd)
- [Atlassian — Adaptive Software Development](https://www.atlassian.com/br/agile/software-development/adaptive-software-development)

