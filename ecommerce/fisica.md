```json
id: int,
pessoa: (identificação de Pessoa: id e/ou identificadoresCivis ou nome),
identificadoresCivis: {
  RG: {
    numero: int | string,
    orgaoExpedidor: string,
    dataExpedicao: Date
  },
  CPF: string | int
},
dataNascimento: Date,
naturalidade: {
  CEP: string | int,
  país: string,
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
},
pai: (identificação de Pessoa: id e/ou identificadoresCivis ou nome),
mãe: (identificação de Pessoa: id e/ou identificadoresCivis ou nome)
```
