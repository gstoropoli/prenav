# ⛵ PréNav — Briefing de Navegação

Dashboard de consulta pré-navegação para velejadores. Um único arquivo HTML, sem backend, sem API keys — funciona em qualquer navegador e pode ser fixado na tela inicial do celular como app.

**Acesse:** https://gstoropoli.github.io/prenav/

## Funcionalidades

- **Previsão 7 dias** estilo Windguru: vento e rajada em nós, direção, temperatura, chuva, nuvens, ondas (altura, período, direção) — com seletor de modelo (GFS, ECMWF, ICON) e de célula de grade (mar/terra)
- **Widget de tempo** estilo iOS, com fita horária e previsão diária expansível
- **Maré**: previsão harmônica local (estações Ubatuba e Cananéia, constantes IO-USP) + modelo global Copernicus, com horários de preamar/baixa-mar
- **Lua e Sol**: fase da lua, iluminação, nascer/pôr, crepúsculos civil e náutico
- **Almanaque náutico**: AHar (GHA ♈), AHG e declinação do Sol a cada 2h UT
- **Estrelas de navegação**: as 57 estrelas + Polaris com Dec, SHA, AHG e altura/azimute calculados para seu local (J2000 + precessão)
- **Boletins por METAREA**: detecta a região e mostra as fontes oficiais (Meteoromarinha/Marinha no Brasil, NOAA, Météo-France etc.)
- **SOS**: painel de emergência guiado passo a passo, com roteiro MAYDAY preenchido com sua posição, telefone regional de socorro e contatos técnicos — funciona offline

## Uso

Busque uma cidade/porto, use o GPS ou digite coordenadas (`-23.78, -45.36`). Preferências, favoritos e dados da embarcação ficam salvos no aparelho (localStorage) — nada é enviado a servidores próprios.

## Fontes de dados

- Meteorologia e ondas: [Open-Meteo](https://open-meteo.com) (GFS/ECMWF/ICON, MFWAM, Copernicus Marine)
- Constantes de maré: Mesquita & Harari (1983), IO-USP
- Efemérides: calculadas localmente (algoritmos de Meeus/SunCalc)

## Aviso

Ferramenta de **planejamento**. Não substitui as publicações oficiais da DHN/Marinha do Brasil nem os boletins dos coordenadores METAREA. Decisões de navegação são responsabilidade exclusiva do comandante.

## Licença

[MIT](LICENSE) © 2026 Gabriel Storopoli
