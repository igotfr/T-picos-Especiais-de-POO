nome | RG | CPF | Telefone | Endereço | 

```mongo
nome: string,
id: int,
identificadoresCivis: {
  RG: {
    numero: int | string,
    orgaoExpedidor: string,
    dataExpedicao: Date,
  },
  CPF: string | int
},
dataNascimento: Date,
naturalidade
telefones: [string | int],
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
  }
],
pai: (identificação de Pessoa, id e/ou identificadoresCivis ou nome),
mãe: (identificação de Pessoa, id e/ou identificadoresCivis ou nome)
```
