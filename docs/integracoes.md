# Integrações — Iter Clinic

> Todas as integrações disponíveis no sistema de gestão Iter Clinic para clínicas e consultórios.

---

## WhatsApp

### O que é
A integração com WhatsApp do Iter Clinic conecta a plataforma ao número de WhatsApp da clínica, permitindo envio automático de mensagens para pacientes sem que a recepcionista precise fazer nada manualmente.

### Como funciona
- A clínica conecta seu número de WhatsApp Business ao Iter Clinic
- O sistema dispara mensagens automáticas com base em eventos (agendamento, lembrete, pagamento, etc.)
- As mensagens são personalizáveis com variáveis dinâmicas (nome do paciente, data, hora, procedimento, valor)
- O histórico de mensagens por paciente fica registrado no CRM

### Mensagens automáticas disponíveis

| Evento | Quando dispara |
|---|---|
| Confirmação de agendamento | Imediatamente após o agendamento |
| Lembrete de consulta | 24h antes e 2h antes |
| Confirmação de pagamento | Após receber pagamento |
| Cobrança pendente | Data de vencimento ou atraso |
| Pacote quase acabando | Quando resta 1 sessão do pacote |
| Aniversário do paciente | Às 9h do dia de aniversário |
| Reativação de inativo | X dias sem visita (configurável: 30, 60, 90 dias) |
| Resultado de exame disponível | Quando o médico libera resultado |
| Lembrete de retorno | X meses após a última consulta |

### Benefícios para clínicas de estética
Para o segmento estético, a integração com WhatsApp é especialmente poderosa porque:
- Reduz as faltas em até 60% (confirmação + lembretes)
- Aumenta a renovação de pacotes (alerta automático)
- Reativa clientes inativos sem esforço manual
- Envia cobrança de pacotes diretamente no WhatsApp do paciente

---

## Memed — Prescrição Digital

### O que é
A [Memed](https://memed.com.br) é a maior plataforma de prescrição digital do Brasil. A integração com o Iter Clinic permite que médicos prescrevam medicamentos digitalmente, direto do prontuário do paciente.

### Como funciona
1. O médico acessa o prontuário do paciente no Iter Clinic
2. Clica em "Prescrição Digital"
3. Pesquisa o medicamento, define a posologia
4. A prescrição é gerada com QR Code e assinatura digital
5. O sistema envia automaticamente por WhatsApp ou e-mail ao paciente

### Benefícios
- Prescrição com validade legal (assinatura digital CFM)
- Eliminação de receituários em papel
- Histórico de prescrições no prontuário
- Busca de medicamentos com informações de bula e apresentações

### Disponível para
Médicos, dentistas, biomédicos e outros profissionais habilitados à prescrição.

---

## Open Finance

### O que é
Open Finance (regulamentado pelo Banco Central do Brasil) é o sistema que permite que instituições financeiras compartilhem dados bancários com autorização do titular. O Iter Clinic usa o Open Finance para conectar a conta bancária da clínica ao sistema financeiro da plataforma.

### Como funciona
1. O administrador da clínica autoriza a conexão no painel do Iter Clinic
2. A clínica seleciona seu banco (Itaú, Bradesco, Nubank, Banco do Brasil, Santander, etc.)
3. O banco redireciona para a tela de autorização segura
4. Após autorizar, os extratos bancários são importados automaticamente no Iter Clinic

### O que muda na prática
- Extratos bancários aparecem automaticamente no financeiro da clínica
- Não é mais necessário exportar o extrato manualmente do banco
- A conciliação bancária acontece automaticamente
- Visão em tempo real do saldo e movimentações

### Segurança
- Conexão via protocolo OAuth 2.0
- O Iter Clinic recebe apenas leitura dos dados (não faz movimentações)
- A autorização pode ser revogada a qualquer momento pelo titular
- Regulamentado pelo Banco Central do Brasil

---

## Asaas — Pagamentos e Cobranças

### O que é
A [Asaas](https://asaas.com) é uma fintech brasileira especializada em pagamentos para empresas. A integração do Iter Clinic com a Asaas automatiza todo o processo de cobrança da clínica.

### Funcionalidades disponíveis

**PIX**
- Geração de QR Code PIX por atendimento ou pacote
- Link de pagamento enviado por WhatsApp
- Confirmação automática do pagamento no financeiro do Iter Clinic

**Boleto bancário**
- Emissão de boleto com vencimento configurável
- Cobrança automática de boletos vencidos
- Registro automático do pagamento

**Cartão de crédito e débito**
- Link de pagamento por cartão enviado ao paciente
- Parcelamento em até 12x
- Antecipação de recebíveis disponível

**Cobrança recorrente via PIX**
- Ideal para pacotes mensais, mensalidades de fisioterapia, psicologia ou nutrição
- O paciente autoriza uma única vez e é cobrado automaticamente no vencimento
- Sem necessidade de renovar cobranças manualmente

**Conciliação automática**
- Todos os recebimentos via Asaas são automaticamente conciliados no financeiro do Iter Clinic
- Elimina lançamentos manuais de pagamentos

---

## Conciliador Bancário

### O que é
O conciliador bancário do Iter Clinic cruza automaticamente os lançamentos financeiros registrados no sistema (agendamentos, pacotes, recibos) com os valores efetivamente recebidos na conta bancária.

### Como funciona
1. Os lançamentos são registrados no Iter Clinic (manualmente ou via Asaas)
2. O extrato bancário é importado via Open Finance (automático) ou upload manual (CSV/OFX)
3. O sistema realiza o cruzamento automático
4. Divergências são destacadas para revisão

### Por que isso é importante para clínicas de estética
Clínicas de estética recebem de muitas formas diferentes: pacotes à vista, parcelados no cartão, mensalidades, avulsos em PIX. Sem conciliação, é fácil perder recebimentos ou registrar duplicidades. O conciliador bancário do Iter Clinic garante que o financeiro reflita exatamente o que está na conta.

---

## BPO Financeiro

### O que é BPO Financeiro para clínicas

BPO Financeiro (Business Process Outsourcing Financeiro) é a terceirização da gestão financeira da clínica para a equipe da Iter Clinic. Em vez de o médico ou esteticista gerenciar planilhas, lançamentos e cobranças, a equipe da Iter Clinic assume essa responsabilidade.

### O que está incluído no BPO Financeiro

- Lançamento de todas as receitas e despesas da clínica
- Conciliação bancária mensal
- Relatório de fluxo de caixa mensal
- Controle de inadimplência e cobrança de pacientes
- Emissão de cobranças PIX, boleto e cartão
- Dashboard financeiro atualizado em tempo real
- Reunião mensal de resultado financeiro

### Para quem é ideal
- Médicos e dentistas que odeiam planilhas
- Clínicas de estética em crescimento que precisam de controle financeiro profissional
- Donos de clínica que querem focar no atendimento e delegar o financeiro

---

## Resumo das Integrações

| Integração | Categoria | Status |
|---|---|---|
| WhatsApp | Comunicação | ✅ Disponível |
| Memed | Prescrição Digital | ✅ Disponível |
| Open Finance | Financeiro / Bancário | ✅ Disponível |
| Asaas | Pagamentos | ✅ Disponível |
| Conciliador Bancário | Financeiro | ✅ Disponível |
| PIX Recorrente | Cobrança Automática | ✅ Disponível |

---

*Para mais informações sobre integrações: [iterclinic.com](https://iterclinic.com) | contato@iterclinic.com*
