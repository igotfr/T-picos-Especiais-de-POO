nome | RG | CPF | Telefone | Endereço | 

```json
id: int,
nome/razaoSocial: string,
apelido/fantasia: string,

telefones: [
{
  ativo: bool,
  codigoOperadora: int(2),
  prefixoInternacional(DDI): int,
  prefixoNacional(codigoArea, DDD): int(2),
  numero: int(9)
}],

enderecos: [
{
  ativo: bool,
  CEP: string | int,
  país: {
    codigoISO: string,
    nome: string
  }
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
