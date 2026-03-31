# PetLife

<p align="center">
	<img src="img/logo.svg" alt="Logo PetLife" width="220" />
</p>

<p align="center">
	Landing page institucional para clínica veterinária, pet shop e farmácia pet.
</p>

<p align="center">
	<img alt="Status" src="https://img.shields.io/badge/status-conclu%C3%ADdo-2ea44f" />
	<img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" />
	<img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" />
	<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=111" />
</p>

## Sobre o projeto

O **PetLife** é um projeto front-end estático criado para praticar fundamentos de desenvolvimento web com foco em:

- Estrutura semântica com HTML5
- Estilização e layout com CSS3
- Interatividade com JavaScript puro

O site apresenta uma página institucional com seções de início, clínica, farmácia/pet shop, dúvidas frequentes e rodapé com contato.

## Funcionalidades

- Navegação por âncoras no menu principal
- Seções informativas com conteúdo de clínica e farmácia
- FAQ com comportamento expansível/colapsável
- Botão de contato direto via WhatsApp
- Estrutura visual moderna para apresentação de serviços

## Preview

> Dica: após clonar o projeto, abra o arquivo `index.html` no navegador para visualizar o layout completo.

<p align="center">
	<img src="img/start-img.svg" alt="Ilustração da seção inicial" width="420" />
	<img src="img/clinic-img.svg" alt="Ilustração da seção clínica" width="320" />
</p>

## Tecnologias utilizadas

- **HTML5** para estrutura e semântica
- **CSS3** para tipografia, cores, layout e componentes visuais
- **JavaScript (ES5/ES6)** para interação no bloco de dúvidas
- **Google Fonts** para as famílias tipográficas do projeto

## Estrutura de pastas

```text
PetLife/
├── img/
│   ├── arrow-down.svg
│   ├── clinic-img.svg
│   ├── faq-img.svg
│   ├── Ionic-Ionicons-Paw-sharp.512.png
│   ├── logo-white.svg
│   ├── logo.svg
│   ├── shape.svg
│   ├── shop-img.svg
│   └── start-img.svg
├── index.html
├── index.css
├── index.js
└── README.md
```

## Como executar localmente

### 1. Clonar o repositório

```bash
git clone https://github.com/Guilherme-R-Santos/PetLife.git
```

### 2. Acessar a pasta do projeto

```bash
cd PetLife
```

### 3. Abrir no navegador

Opção A:

- Abra o arquivo `index.html` diretamente no navegador.

Opção B (recomendado para desenvolvimento):

- Use uma extensão como **Live Server** no VS Code para recarregamento automático.

## Lógica JavaScript

A interatividade do FAQ é baseada em alternância de classe CSS ao clicar em cada item de dúvida.

```javascript
var elementosDuvida = document.querySelectorAll('.duvida')

elementosDuvida.forEach(function (duvida) {
	duvida.addEventListener('click', function () {
		duvida.classList.toggle('ativa')
	})
})
```

Quando a classe `ativa` é aplicada, o CSS expande o conteúdo da resposta.


