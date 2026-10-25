# apuracao-dados

Histórico da apuração das Eleições 2026 (Presidente, 2º turno) usado em https://apuracao.lenderson.com.br.

O TSE não publica histórico. Estes arquivos são snapshots reais do arquivo público do TSE
(`resultados.tse.jus.br`), coletados a cada 10 minutos desde o início da nossa coleta. Nenhum ponto é interpolado.

- `history/br.json`: Brasil
- `history/<uf>.json`: cada UF (ex.: `sp.json`)
- `history/index.json`: quantidade de pontos por arquivo

Cada ponto: `{ t (data/hora da totalização do TSE), collectedAt, pctSecoesTotalizadas, candidates: [{ n, nm, pvap, vap }] }`.
