nome | RG | CPF | Telefone | Endereço | 

```json
nome: string,
id: int,
identificadoresCivis: {
  RG: {
    numero: int | string,
    orgaoExpedidor: string,
    dataExpedicao: Date
  },
  CPF: string | int
},
telefones: [
{
  codigoOperadora: int(2),
  prefixoInternacional(DDI): int,
  prefixoNacional(codigoArea, DDD): int(2),
  numero: int(9)
}
],
dataNascimento: Date,
naturalidade: {
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
}
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
pai: (identificação de Pessoa: id e/ou identificadoresCivis ou nome),
mãe: (identificação de Pessoa: id e/ou identificadoresCivis ou nome)
```
