
# 🚢 Batalha Naval (C)

Projeto acadêmico em **linguagem C** atendendo aos critérios do tema:
- uso de **vetores e matrizes** (tabuleiro 10x10);
- **loops aninhados** e **condicionais**;
- **habilidades com áreas de efeito** (cruz, cone, octógono);
- jogo **Humano × IA** via terminal.

> Ideal para submissão em repositório GitHub da disciplina.

## Como compilar e executar

### Linux / macOS (gcc)
```bash
make        # gera o executável `batalha`
./batalha
```

### Windows (MinGW)
```bash
gcc src/main.c -o batalha -O2
batalha.exe
```

## Regras e documentação
- 📄 `docs/regras.md` — regras do jogo e tamanhos de navios.
- 📄 `docs/manual.md` — como jogar e usar as habilidades.

## Estrutura
```
batalha-naval-c/
├─ src/
│  └─ main.c
├─ docs/
│  ├─ regras.md
│  └─ manual.md
├─ tests/
├─ .gitignore
├─ LICENSE
├─ Makefile
└─ README.md
```

## Funcionalidades
- Tabuleiro **10×10** (`int board[10][10]`).
- Posicionamento automático de navios.
- Ataque simples por coordenadas (ex.: `B7`).
- **Habilidades** (1 uso cada):
  - **Cruz (+)** — raio 2.
  - **Cone** — direção `U/D/L/R`, profundidade 3.
  - **Octógono** (aprox. usando distância de Manhattan) — raio 2.
- Vitória quando todos os navios inimigos forem destruídos.

## Repositório
O código completo está disponível em:  
[https://github.com/jeffdomioliveira/batalha-naval-c](https://github.com/jeffdomioliveira/batalha-naval-c)

## Créditos
Feito para fins educacionais. Licença MIT.
