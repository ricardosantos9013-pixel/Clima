# ⛈️ Clima Alerta · Notícias, Rádios & Rodovias

Aplicação web (PWA) para acompanhamento de condições meteorológicas, radar de chuva, rádios jornalísticas ao vivo, risco de queda de energia, trânsito urbano e ocorrências em rodovias em tempo real.

## ✨ Funcionalidades

- **Clima e previsão:** Temperatura atual, sensação térmica, umidade, vento, rajadas, chuva, pressão, visibilidade, previsão hora a hora e previsão para 7 dias (via Open-Meteo).
- **Radar de chuva:** Camada interativa no mapa (via RainViewer) com modos **Local**, **Estado SP** e **Brasil**, controle de linha do tempo e marcador da cidade.
- **Rodovias e trânsito em tempo real:** Coleta notícias e ocorrências de fontes públicas, concessionárias e imprensa (ex.: **ARTESP / DER**, **Entrevias**, **Eixo SP**, **CART**, **ViaRondon**, **Rodovias do Tietê**, **Ecovias** e portais de notícias), sem dados simulados.
- **Rádios ao vivo:** Player integrado com controle de volume, mudo e *Sleep Timer* (com *fade* opcional).
- **Risco de energia e alertas:** Estimativa de probabilidade de queda de energia com base em vento, rajadas, chuva e tempestade, identificação da distribuidora regional, registros locais e histórico em IndexedDB (com backup opcional via GitHub Gist).
- **Favoritos e busca de cidades:** Alternância entre localização atual (GPS), busca de cidades e lista de favoritos.

## 🚀 Como usar

1. Baixe ou clone o repositório.
2. Abra o arquivo `index.html` em um navegador moderno (ou sirva via servidor HTTP local).
3. Para suporte offline completo como PWA, baixe o `sw.js` pela tela de **Configurações (⚙️)**, coloque na mesma pasta do `index.html` e recarregue a página.

## ⚙️ Configuração opcional (Proxy / ARTESP)

Na janela de **Configurações (⚙️)** do aplicativo, você pode informar:
- **URL de proxy** (por exemplo, Cloudflare Worker) para intermediar requisições ou expor endpoints como `/artesp/ocorrencias`.
- **Distribuidora de energia** (automática pela localização ou manual).
- **Raio de alerta** e preferências de notificação / *Sleep Timer*.

## 📌 Aviso

As informações de rodovias, trânsito e notícias dependem da disponibilidade dos feeds e serviços externos consultados no momento. Em deslocamentos, consulte sempre os canais oficiais e a sinalização na via.
