# dados

Cópias congeladas dos dados usados no notebook. O notebook procura aqui primeiro; se estiver
rodando no Colab (onde só o `.ipynb` é aberto), pega os mesmos arquivos por
`raw.githubusercontent.com`; e só então tenta a fonte original.

| Arquivo | O que é | Fonte original |
|---|---|---|
| `temp_1000mb_lat37N_lon120W_series_only.dat` | T diária em 1000 hPa, 37°N/120°W, 1979–2010, em K (11 680 dias, calendário de 365 dias). **É a série que os exercícios do CLIVAC mandam usar.** | `clivac.eri.ucsb.edu/wp-content/uploads/` |
| `norm.daily.ao.cdas.z1000.19500101_current.csv` | Índice AO (Oscilação Ártica) diário, normalizado, 1950–presente | `ftp.cpc.ncep.noaa.gov/cwlinks/` |
| `norm.daily.aao.cdas.z700.19790101_current.csv` | Índice AAO (Oscilação Antártica) diário, normalizado, 1979–presente | `ftp.cpc.ncep.noaa.gov/cwlinks/` |

Baixados em 2026-09-08. Os índices do CPC são atualizados diariamente na fonte: a cópia daqui é
o que garante que os números discutidos em aula sejam reproduzíveis, mas ela **envelhece** — para
trabalho de verdade, use a fonte original.
