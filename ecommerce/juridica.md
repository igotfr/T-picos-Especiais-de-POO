id: int,
pessoa: (identificação de Pessoa: id e/ou identificadoresCivis ou nome),
identificadores: {
  CNPJ: int | string,
  IE: int | string
},
razãoSocial: string,
fantasia: string,
contribuinte: {
  x: bool,
  regimeApuracao: string
}
