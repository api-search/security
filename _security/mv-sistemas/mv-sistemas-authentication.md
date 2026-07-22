---
api_key_in:
- header
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
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mv Sistemas Authentication
name_suffix: Authentication
oauth_flows: []
overview: MV sistemas secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MV sistemas
provider_slug: mv-sistemas
scheme_count: 3
schemes:
- in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/mv-sistemas-clinic-agenda-openapi.yaml
  - openapi/mv-sistemas-clinic-connect-openapi.yaml
  - openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml
  - openapi/mv-sistemas-clinic-patient-audit-openapi.yaml
  - openapi/mv-sistemas-events-openapi.json
  - openapi/mv-sistemas-face-recognition-openapi.json
  - openapi/mv-sistemas-gestao-beneficiarios-openapi.json
  - openapi/mv-sistemas-hub-operadora-openapi.yaml
  - openapi/mv-sistemas-news-openapi.json
  - openapi/mv-sistemas-pendencias-saude-openapi.json
  - openapi/mv-sistemas-performance-schedule-webhook-openapi.yml
  - openapi/mv-sistemas-personal-attendance-openapi.json
  - openapi/mv-sistemas-personal-health-ficha-clinica-openapi.json
  - openapi/mv-sistemas-protocolo-entrada-openapi.json
  - openapi/mv-sistemas-regulacao-openapi.yaml
  - openapi/mv-sistemas-shared-request-openapi.yaml
  - openapi/mv-sistemas-users-openapi.json
  type: apiKey
- description: Token do One Pass
  in: header
  name: one_pass
  parameter: x-authorization
  sources:
  - openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml
  type: apiKey
- description: Token do Clinic com Bearer
  in: header
  name: clinic
  parameter: authorization
  sources:
  - openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml
  type: apiKey
slug: mv-sistemas-authentication
source_filename: mv-sistemas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mv-sistemas-clinic-agenda-openapi.yaml, openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml,\n  openapi/mv-sistemas-clinic-connect-openapi.yaml, openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml,\n  openapi/mv-sistemas-clinic-patient-audit-openapi.yaml, openapi/mv-sistemas-events-openapi.json,\n  openapi/mv-sistemas-face-recognition-openapi.json, openapi/mv-sistemas-gestao-beneficiarios-openapi.json,\n  openapi/mv-sistemas-hub-operadora-openapi.yaml, openapi/mv-sistemas-news-openapi.json, openapi/mv-sistemas-pendencias-saude-openapi.json,\n  openapi/mv-sistemas-performance-schedule-webhook-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/mv-sistemas-clinic-agenda-openapi.yaml\n  - openapi/mv-sistemas-clinic-connect-openapi.yaml\n  - openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml\n\
  \  - openapi/mv-sistemas-clinic-patient-audit-openapi.yaml\n  - openapi/mv-sistemas-events-openapi.json\n  - openapi/mv-sistemas-face-recognition-openapi.json\n  - openapi/mv-sistemas-gestao-beneficiarios-openapi.json\n  - openapi/mv-sistemas-hub-operadora-openapi.yaml\n  - openapi/mv-sistemas-news-openapi.json\n  - openapi/mv-sistemas-pendencias-saude-openapi.json\n  - openapi/mv-sistemas-performance-schedule-webhook-openapi.yml\n  - openapi/mv-sistemas-personal-attendance-openapi.json\n  - openapi/mv-sistemas-personal-health-ficha-clinica-openapi.json\n  - openapi/mv-sistemas-protocolo-entrada-openapi.json\n  - openapi/mv-sistemas-regulacao-openapi.yaml\n  - openapi/mv-sistemas-shared-request-openapi.yaml\n  - openapi/mv-sistemas-users-openapi.json\n- name: one_pass\n  type: apiKey\n  in: header\n  parameter: x-authorization\n  description: Token do One Pass\n  sources:\n  - openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml\n- name: clinic\n  type: apiKey\n  in: header\n  parameter:\
  \ authorization\n  description: Token do Clinic com Bearer\n  sources:\n  - openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/authentication/mv-sistemas-authentication.yml
summary_line: apiKey · 3 schemes
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
