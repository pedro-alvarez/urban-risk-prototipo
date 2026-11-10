# Protótipo – Urban Risk Intelligence Platform (Engenharia de Software)

Global Solution 2026.2 | Turma 3ECR | 554603 – Pedro Alvarez Certo | 555143 – Gustavo Demeis Peres

Protótipo funcional e navegável (HTML + CSS + JavaScript, sem dependências e sem instalação) com 10 telas:
painel de acompanhamento, mapa de eventos, lista de alertas, detalhe do evento, central de notificações,
registro comunitário de ocorrência, origem e confiança dos dados, saúde das fontes, preferências e privacidade (LGPD)
e seletor de perfil (morador, agente da Defesa Civil e operador de serviço público).

## Como executar

Abra `index.html` em qualquer navegador (clique duas vezes no arquivo). Não há servidor nem build.

Links diretos para cada tela: `index.html#painel`, `#mapa`, `#alertas`, `#notificacoes`, `#registrar`, `#confianca`, `#fontes`, `#privacidade` e `#detalhe/EV-1042`.

## Fluxo principal para testar

1. **Painel** → clique em um alerta prioritário.
2. No **detalhe**, veja origem, evidências e confiança (RN-01). Com o perfil “Agente da Defesa Civil”, use as ações do ciclo de vida (validar → confirmar → emitir alerta → monitorar → encerrar).
3. Abra a **Central de notificações**: o alerta emitido aparece lá.
4. Troque o perfil para “Morador” e use **Registrar ocorrência**: o relato entra como “Reportado” com confiança 40%.
5. Veja **Origem e confiança**, **Saúde das fontes** e **Preferências e privacidade**.

## Publicar para o link do relatório (GitHub Pages)

1. Crie um repositório no GitHub e envie esta pasta (ou o repositório todo).
2. Em *Settings → Pages*, escolha a branch e a pasta que contém `index.html`.
3. Use o endereço gerado como “link do protótipo” no PDF e teste em janela anônima.

## Observações

- Os dados são fictícios (bairro de exemplo “Nova Aurora”) e ficam apenas na memória do navegador.
- As regras RN-01 a RN-04 do documento estão implementadas em JavaScript (confiança, nível de confiança, prioridade e restrição de alerta). O risco de cada evento de exemplo (RN-05) já vem classificado nos dados fictícios.
