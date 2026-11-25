# 226182_226232_226373_226352_mareemprego

Maré Emprego – ofertas de trabalho em todo o Portugal.

## Como abrir o site

As ofertas são carregadas do ficheiro `ofertas.json` com `fetch`. Por isso, o site tem de ser aberto através de um servidor (abrir o `.html` diretamente com duplo clique faz o navegador bloquear o carregamento).

```bash
python3 -m http.server 8000
# depois abrir http://localhost:8000/Mare%20emprego.html
```

Também funciona com a extensão Live Server do VS Code ou no GitHub Pages.

## Ofertas (`ofertas.json`)

Cada oferta é um objeto com:

| Campo | Significado |
| --- | --- |
| `id` | Número único |
| `t` | Título da função |
| `c` | Empresa |
| `m` | Cidade (tem de existir na lista de cidades do site) |
| `a` | Área |
| `k` | Tipo de contrato |
| `r` | Regime (Presencial, Híbrido…) |
| `salarioMin`, `salarioMax` | Salário em €/mês |
| `d` | Há quantos dias foi publicada |
| `p` | Descrição |
| `q` | Lista de requisitos |

## Privacidade

O perfil, a foto, as ofertas guardadas, as candidaturas e as cartas de apresentação ficam apenas no `localStorage` do navegador. No separador Perfil é possível exportar tudo para um ficheiro JSON ou apagar todos os dados.
