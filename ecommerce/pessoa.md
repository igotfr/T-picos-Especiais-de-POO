nome | RG | CPF | Telefone | Endereço | 

```json
id: int,
nome/razaoSocial: string(>=2),
apelido/fantasia: string(>=2),
```
<details>
  <summary><pre>
telefones: ?[
{
  ativo: bool,
  codigoOperadora: int?(algarismos: 2),
  prefixoInternacional(DDI): int?(algarismos: 1:3),
  prefixoNacional(codigoArea, DDD): int?(algarismos: 2),
  numero(SN - Subscriber Number): int(algarismos: 6:9)
}],</pre></summary>

  <pre>
Implementação:
  1ª Opção: cada chave-valor do Javascript Object pode corresponder a um input
  2ª Opção: um único input para cada telefone, o valor é dividido em substrings cujos valores são alocados às chaves
  correspondentes através de uma função
    pattern input: 

Links: https://www.cm.com/blog/how-to-format-international-telephone-numbers/
  </pre>
</details>

```json
enderecos: ?[
{
  ativo: bool,
```
<details>
  <summary><code>CEPbrasileiro: string() | int(8),</code></summary>

  https://www.mbi.com.br/mbi/biblioteca/paises/codigo-postal/
</details>

  país: {
    codigoISO2: string(2),
    codigoISO3: string(3),
    nome: string
  }
```json
  UF: {
    idIBGE: int,
    sigla: string(2),
    nome: string
  },
  municipio: {
    idIBGE: int,
    nome: string
  }
  bairro/distrito: string,
  logradouro: {
    tipo: string,
    nome: string
  },
  numero: int,
  quadra: int,
  lote: int,
  complemento: string
}],
```
