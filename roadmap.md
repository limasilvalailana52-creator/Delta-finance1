# Roadmap — Delta Finance

## Fase 1 — versão local
- [x] Painel responsivo em tema escuro
- [x] Cadastro local de ganhos, gastos e investimentos
- [x] Extrato com filtros e busca
- [x] Status pago/pendente
- [x] Relatórios com visualizações
- [x] Perfil local e exportação CSV

## Fase 2 — nuvem e autenticação
- [ ] Criar projeto Supabase
- [ ] Implementar cadastro/login e recuperação de senha
- [ ] Criar tabelas com RLS por usuário
- [ ] Migrar operações do localStorage para banco autenticado
- [ ] Oferecer importação/exportação e migração de dados locais

## Fase 3 — WhatsApp
- [ ] Configurar WhatsApp Cloud API e webhook HTTPS
- [ ] Validar assinatura do webhook e evitar duplicação de eventos
- [ ] Vincular número de WhatsApp a usuário após confirmação
- [ ] Processar texto e áudio com tratamento de privacidade
- [ ] Pedir confirmação antes de gravar mensagens ambíguas
- [ ] Responder consultas de saldo usando os dados do usuário autenticado

## Segurança para produção
- Nunca colocar chaves secretas no JavaScript do navegador ou no GitHub.
- Validar entrada de dados e origem de webhooks.
- Aplicar políticas de acesso no banco.
- Evitar registrar conteúdo financeiro nos logs.
- Testar cópias de segurança, exclusão de conta e recuperação de dados.
