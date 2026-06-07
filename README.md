<div align="center">

# Validador de CPF

*Implementação do algoritmo oficial da Receita Federal em Python puro*

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/status-concluído-2ea44f?style=flat)

</div>

---

## Sobre

Valida um CPF calculando seus dois dígitos verificadores a partir dos nove primeiros dígitos e os compara com os dígitos originais — seguindo exatamente o algoritmo definido pela Receita Federal do Brasil.

---

## Como funciona

O algoritmo opera em duas etapas:

**1ª etapa — 10º dígito**
> Multiplica os 9 primeiros dígitos por pesos decrescentes (10 → 2), soma os resultados e aplica `(soma × 10) % 11`. Se o resultado for maior que 9, o dígito é `0`.

**2ª etapa — 11º dígito**
> Repete o processo com os 10 dígitos anteriores e pesos de 11 → 2.

Se ambos coincidirem com os dígitos originais do CPF → ✅ válido.

---

## Como executar

```bash
git clone https://github.com/seu-usuario/validador-cpf.git
cd validador-cpf
python validador_cpf.py
```

**Exemplo de saída:**
```python
cpf = "16804508084"
# → 8 4  ✅
```

---

## Tecnologias

`Python 3` · sem dependências externas

---

<div align="center">

**Carlos** — estudante de Python com foco em segurança da informação

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/seu-perfil)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/seu-usuario)

</div>
