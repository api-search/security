---
api_specs:
- filename: mv-sistemas-clinic-agenda-openapi.yaml
  format: yaml
  label: Clinic Agenda
  slug: clinic-agenda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-agenda-openapi.yaml
- filename: mv-sistemas-clinic-connect-attendance-openapi.yaml
  format: yaml
  label: 'Clinic Connect : Atendimento'
  slug: clinic-connect-atendimento
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml
- filename: mv-sistemas-clinic-connect-openapi.yaml
  format: yaml
  label: Clinic Connect
  slug: clinic-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-openapi.yaml
- filename: mv-sistemas-clinic-connect-performance-schedule-openapi.yml
  format: yaml
  label: Clinic Connect - Agendamento de performance API
  slug: clinic-connect-agendamento-de-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml
- filename: mv-sistemas-clinic-patient-audit-openapi.yaml
  format: yaml
  label: 'Clinic : Auditoria de dados de saúde do paciente'
  slug: clinic-auditoria-de-dados-de-saúde-do-paciente
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-patient-audit-openapi.yaml
- filename: mv-sistemas-events-openapi.json
  format: json
  label: API para Gestão de Eventos
  slug: api-para-gestão-de-eventos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-events-openapi.json
- filename: mv-sistemas-face-recognition-openapi.json
  format: json
  label: Reconhecimento Facial
  slug: reconhecimento-facial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-face-recognition-openapi.json
- filename: mv-sistemas-gestao-beneficiarios-openapi.json
  format: json
  label: Gestão de Dados Cadastrais dos Beneficiários
  slug: gestão-de-dados-cadastrais-dos-beneficiários
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-gestao-beneficiarios-openapi.json
- filename: mv-sistemas-hub-operadora-openapi.yaml
  format: yaml
  label: Integração Hub Operadora
  slug: integração-hub-operadora
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-hub-operadora-openapi.yaml
- filename: mv-sistemas-news-openapi.json
  format: json
  label: News - Global Health
  slug: news-global-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-news-openapi.json
- filename: mv-sistemas-pendencias-saude-openapi.json
  format: json
  label: Gestão de Pendências de Saúde
  slug: gestão-de-pendências-de-saúde
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-pendencias-saude-openapi.json
- filename: mv-sistemas-performance-schedule-webhook-openapi.yml
  format: yaml
  label: Webhook - Agendamento de performance
  slug: webhook-agendamento-de-performance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-performance-schedule-webhook-openapi.yml
- filename: mv-sistemas-personal-attendance-openapi.json
  format: json
  label: 'Personal Health : Atendimentos'
  slug: personal-health-atendimentos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-personal-attendance-openapi.json
- filename: mv-sistemas-personal-health-ficha-clinica-openapi.json
  format: json
  label: 'Personal Health : Ficha Clínica'
  slug: personal-health-ficha-clínica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-personal-health-ficha-clinica-openapi.json
- filename: mv-sistemas-protocolo-entrada-openapi.json
  format: json
  label: Protocolo de Entrada
  slug: protocolo-de-entrada
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-protocolo-entrada-openapi.json
- filename: mv-sistemas-regulacao-openapi.yaml
  format: yaml
  label: 'Clinic Connect : Regulação'
  slug: clinic-connect-regulação
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-regulacao-openapi.yaml
- filename: mv-sistemas-shared-request-openapi.yaml
  format: yaml
  label: Compartilhamento de Dados
  slug: compartilhamento-de-dados
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-shared-request-openapi.yaml
- filename: mv-sistemas-users-openapi.json
  format: json
  label: Users - Global Health
  slug: users-global-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-users-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mvsistemas.com.br
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: globalhealth.mv
  spf: false
hosts:
- host: www.mvsistemas.com.br
  https: false
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.globalhealth.mv
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api-hml.globalhealth.mv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mv Sistemas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MV sistemas, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MV sistemas
provider_slug: mv-sistemas
slug: mv-sistemas-domain-security
source_filename: mv-sistemas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mvsistemas.com.br\n  https: false\n- host: api.globalhealth.mv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: api-hml.globalhealth.mv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mvsistemas.com.br\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: globalhealth.mv\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/security/mv-sistemas-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Health IT
- Hospital
- Clinic
- Health Insurance
- FHIR
- Brazil
- Patient Data
- Scheduling
- Biometrics
---
