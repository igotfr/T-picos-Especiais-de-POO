nome | RG | CPF | Telefone | Endereço | 

```json
nome: string,
id: int,

telefones: [
{
  codigoOperadora: int(2),
  prefixoInternacional(DDI): int,
  prefixoNacional(codigoArea, DDD): int(2),
  numero: int(9)
}],


enderecos: [
{
  ativo: bool,
  CEP: string | int,
  estado: string,
  cidade: string,
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
