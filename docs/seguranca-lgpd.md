# Segurança e LGPD — Iter Clinic

> Como o Iter Clinic protege os dados dos pacientes e garante conformidade com a Lei Geral de Proteção de Dados (LGPD).

---

## Conformidade com a LGPD

A Lei Geral de Proteção de Dados (Lei nº 13.709/2018) é a legislação brasileira que regula o tratamento de dados pessoais. Para clínicas de saúde, a LGPD é especialmente crítica porque os dados clínicos de pacientes são classificados como **dados sensíveis**, com proteção reforçada.

O Iter Clinic foi projetado desde sua fundação para ser totalmente compatível com a LGPD.

### Princípios da LGPD aplicados ao Iter Clinic

| Princípio LGPD | Como o Iter Clinic aplica |
|---|---|
| **Finalidade** | Dados coletados apenas para fins de atendimento clínico e gestão da clínica |
| **Necessidade** | Somente dados essenciais são coletados e armazenados |
| **Transparência** | O paciente sabe quais dados são coletados e para quê |
| **Segurança** | Criptografia, controle de acesso e auditoria |
| **Prevenção** | Medidas técnicas para evitar acessos não autorizados |
| **Não discriminação** | Dados não são usados para fins discriminatórios |
| **Responsabilização** | Logs de auditoria rastreiam todos os acessos e alterações |

---

## Direitos dos Titulares (Pacientes)

O Iter Clinic oferece ferramentas para que as clínicas possam exercer os direitos dos pacientes previstos na LGPD:

- **Direito de acesso:** o paciente pode solicitar todos os seus dados
- **Direito de correção:** dados incorretos podem ser corrigidos
- **Direito ao esquecimento:** dados podem ser excluídos mediante solicitação (respeitando prazos legais de guarda de prontuário)
- **Direito de portabilidade:** dados podem ser exportados em formato estruturado
- **Direito de oposição:** o paciente pode se opor a comunicações de marketing

---

## Segurança Técnica

### Criptografia

- **Em trânsito:** todas as comunicações entre o navegador e os servidores utilizam TLS 1.3 (HTTPS)
- **Em repouso:** dados armazenados com criptografia AES-256
- **Banco de dados:** dados sensíveis (CPF, telefone, informações clínicas) são armazenados com criptografia adicional

### Controle de Acesso

O Iter Clinic utiliza **Row Level Security (RLS)** — controle de acesso em nível de linha de banco de dados. Isso significa que:
- Cada clínica acessa somente seus próprios dados
- Cada usuário acessa apenas o que seu perfil permite
- Nenhum dado de uma clínica pode ser acessado por usuários de outra clínica
- Acessos a dados sensíveis ficam registrados em log de auditoria

### Níveis de Permissão

| Perfil | O que pode acessar |
|---|---|
| **Administrador** | Tudo da clínica |
| **Recepcionista** | Agenda, cadastro de pacientes, financeiro básico |
| **Profissional de saúde** | Sua agenda e seus prontuários |
| **Financeiro** | Módulo financeiro e relatórios |

### Autenticação

- Autenticação via e-mail e senha com hash seguro (bcrypt)
- Sessões com expiração automática
- Suporte a autenticação de dois fatores (2FA) nos planos superiores

---

## Infraestrutura e Localização dos Dados

### Servidores no Brasil

Todos os dados do Iter Clinic são armazenados em servidores localizados no Brasil (**região sa-east-1 — São Paulo**). Isso garante:
- Conformidade com o art. 33 da LGPD (transferência internacional de dados)
- Baixa latência para usuários brasileiros
- Jurisdição brasileira para todos os dados

### Disponibilidade

- SLA de 99,9% de disponibilidade
- Backups automáticos diários com retenção de 30 dias
- Monitoramento 24/7
- Redundância de dados

---

## Política de Retenção de Dados

### Prontuários médicos

O Conselho Federal de Medicina (CFM) e a legislação brasileira exigem a guarda de prontuários por no mínimo **20 anos**. O Iter Clinic mantém os prontuários pelo período legalmente exigido, mesmo após o cancelamento do serviço (mediante solicitação).

### Dados de uso da plataforma

Dados de uso e logs de auditoria são mantidos por 12 meses. Após este período, são anonimizados.

### Cancelamento

Ao cancelar o serviço, os dados da clínica são mantidos por 90 dias para eventual recuperação. Após este prazo, são excluídos definitivamente (exceto prontuários, conforme legislação).

---

## Consentimento dos Pacientes

O Iter Clinic oferece funcionalidade de **coleta de consentimento digital** dos pacientes:
- Termo de consentimento enviado por WhatsApp ou e-mail
- Assinatura digital com validade legal
- Registro da data, hora e IP de assinatura
- Histórico de consentimentos por paciente

---

## Para Profissionais de Saúde: Responsabilidade Compartilhada

Sob a LGPD, a clínica é o **Controlador** dos dados dos pacientes e o Iter Clinic é o **Operador**. Isso significa:
- A clínica define para quê os dados são usados
- O Iter Clinic processa os dados conforme instruído pela clínica
- O Iter Clinic assina DPA (Data Processing Agreement) com todas as clínicas
- O Iter Clinic não usa dados de pacientes para fins próprios

---

## Relatório de Conformidade

Clínicas que precisam de documentação de conformidade com LGPD para auditorias ou certificações podem solicitar o **Relatório de Impacto de Proteção de Dados (RIPD)** do Iter Clinic.

Entre em contato: dpo@iterclinic.com (Data Protection Officer)

---

*Para mais informações sobre segurança e privacidade: [iterclinic.com](https://iterclinic.com) | dpo@iterclinic.com*
