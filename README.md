# 🏟️ Pokémon Stadium Rental Team Builder

![Status](https://img.shields.io/badge/Status-Completed-success)
![Version](https://img.shields.io/badge/Version-1.0-blue)
![Gen](https://img.shields.io/badge/Gen-1%20(RBY)-red)

Uma ferramenta web interativa e **responsiva** para visualizar, filtrar e montar times com os **Pokémon de Aluguel (Rentals)** do jogo **Pokémon Stadium 1 USA (Nintendo 64)**. Atualmente focado na **Pika Cup (Level 15-20)**.

Desenvolvido para ser acessado facilmente via celular enquanto você joga no console ou emulador.

## Funcionalidades

### Base de Dados Interativa
- **Lista Completa:** Todos os Pokémon de aluguel da Pika Cup.
- **Ordenação:** Classifique por Velocidade (Speed), Ataque, HP, etc.
- **Busca Inteligente:** Filtre por Nome, Tipo (ex: "Fire"), Golpe (ex: "Surf") ou até Fraqueza.

### Mecânicas da Geração 1 (RBY)
- **Tabela de Tipos Gen 1:** O sistema calcula fraquezas e resistências baseadas nas regras originais (ex: Inseto é super efetivo contra Veneno, Gelo é neutro contra Fogo).
- **Indicador de Precisão:** Golpes com **100% de Accuracy** recebem destaque visual (borda dourada + ícone 🎯), essencial para estratégias consistentes no Stadium.
- **Tipagem Original:** Considera os tipos da época (ex: Magnemite é apenas Elétrico).

### Team Builder & Análise
- **Montagem de Time:** Selecione até 6 Pokémon clicando no botão `+`.
- **Barra Fixa:** Visualize seu time atual no rodapé da tela.
- **Dashboard Tático:** Analise seu time com um clique:
    - **Ameaças Defensivas:** Mostra quais tipos dão dano super efetivo na maioria do seu time.
    - **Cobertura Ofensiva:** Mostra quais tipos seus golpes conseguem atingir com vantagem.

### Mobile-First
- Layout totalmente adaptado para telas pequenas.
- Coluna do nome do Pokémon **fixa** na rolagem horizontal.
- Botões e inputs otimizados para toque.

---

## Estrutura do Projeto

O projeto foi separado para facilitar a manutenção e adição de novas Copas (Prime Cup, Poké Cup) no futuro.

```text
/
├── index.html       # Interface, lógica de renderização e Team Builder
├── pokemon_db.js    # Banco de dados (Stats, Moves, Type Chart Gen 1)
└── README.md        # Documentação
