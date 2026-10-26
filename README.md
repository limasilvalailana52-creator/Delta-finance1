# Delta Finance — versão funcional local

Aplicativo web responsivo de controle financeiro, com tema escuro, destaques verde neon e gastos em vermelho. Esta versão funciona sem login, banco remoto ou WhatsApp.

## Funcionalidades
- Painel inicial com saldo mensal, ganhos, gastos e investimentos.
- Cadastro manual de transações, com descrição, categoria, data, valor e status.
- Extrato com filtros por tipo, mês e pesquisa.
- Marcar lançamentos pendentes como pagos e excluir transações.
- Relatórios com gráfico de gastos por categoria, gráfico diário e média diária.
- Análise Delta com insights simulados calculados localmente.
- Perfil com nome personalizado.
- Exportação CSV para backup.
- Armazenamento local por navegador usando `localStorage`.

## Como publicar no GitHub Pages
Este repositório usa um site estático. Para atualizar o site existente:
1. Faça backup da versão atual de `index.html` antes de substituí-la.
2. Abra o repositório GitHub e entre em `index.html`.
3. Use o lápis **Edit this file** ou `Add file → Upload files`.
4. Substitua o conteúdo pelo `index.html` deste pacote e faça commit na branch `main`.
5. Aguarde o GitHub Pages publicar e abra o site. Se não atualizar, recarregue sem cache ou aguarde alguns minutos.

## Estrutura sugerida
```text
Delta-finance1/
├── index.html
├── README.md
└── docs/
    └── roadmap.md
```

## Importante sobre os dados
- Os dados ficam neste navegador/dispositivo e não sincronizam entre celulares.
- Limpar os dados do navegador pode apagar os lançamentos. Exporte CSV periodicamente.
- Esta versão não tem autenticação, criptografia própria, banco em nuvem ou integração com WhatsApp.
- Não use para dados financeiros sensíveis em aparelhos compartilhados.
- O saldo do mês é calculado como ganhos menos gastos e investimentos.
- Insights são heurísticas locais, não aconselhamento financeiro.

## Próximas fases
1. Supabase Auth para cadastro/login.
2. PostgreSQL com Row Level Security e sincronização na nuvem.
3. Importação dos dados locais para a conta autenticada.
4. Back-end para WhatsApp Cloud API, validação de webhook e associação segura do número à conta.
5. Interpretação de texto/áudio com confirmação de dados ambíguos.
