---
api_specs:
- filename: backrow-ai-chat-api-openapi.yml
  format: yaml
  label: Backrow Chat API
  slug: backrow-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-chat-api-openapi.yml
- filename: backrow-ai-credit-transactions-api-openapi.yml
  format: yaml
  label: Backrow Credit Transactions API
  slug: backrow-ai-credit-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-credit-transactions-api-openapi.yml
- filename: backrow-ai-diaries-api-openapi.yml
  format: yaml
  label: Backrow Diaries API
  slug: backrow-ai-diaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-diaries-api-openapi.yml
- filename: backrow-ai-documents-api-openapi.yml
  format: yaml
  label: Backrow Documents API
  slug: backrow-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-documents-api-openapi.yml
- filename: backrow-ai-flashcards-api-openapi.yml
  format: yaml
  label: Backrow Flashcards API
  slug: backrow-ai-flashcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-flashcards-api-openapi.yml
- filename: backrow-ai-health-api-openapi.yml
  format: yaml
  label: Backrow Health API
  slug: backrow-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-health-api-openapi.yml
- filename: backrow-ai-knowledge-state-api-openapi.yml
  format: yaml
  label: Backrow Knowledge State API
  slug: backrow-ai-knowledge-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-knowledge-state-api-openapi.yml
- filename: backrow-ai-lessons-api-openapi.yml
  format: yaml
  label: Backrow Lessons API
  slug: backrow-ai-lessons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-lessons-api-openapi.yml
- filename: backrow-ai-match-video-api-openapi.yml
  format: yaml
  label: Backrow Match Video API
  slug: backrow-ai-match-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-match-video-api-openapi.yml
- filename: backrow-ai-notes-api-openapi.yml
  format: yaml
  label: Backrow Notes API
  slug: backrow-ai-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-notes-api-openapi.yml
- filename: backrow-ai-paths-api-openapi.yml
  format: yaml
  label: Backrow Paths API
  slug: backrow-ai-paths-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-paths-api-openapi.yml
- filename: backrow-ai-pricing-api-openapi.yml
  format: yaml
  label: Backrow Pricing API
  slug: backrow-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-pricing-api-openapi.yml
- filename: backrow-ai-profile-api-openapi.yml
  format: yaml
  label: Backrow Profile API
  slug: backrow-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-profile-api-openapi.yml
- filename: backrow-ai-quizzes-api-openapi.yml
  format: yaml
  label: Backrow Quizzes API
  slug: backrow-ai-quizzes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-quizzes-api-openapi.yml
- filename: backrow-ai-recommendations-api-openapi.yml
  format: yaml
  label: Backrow Recommendations API
  slug: backrow-ai-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-recommendations-api-openapi.yml
- filename: backrow-ai-recordings-api-openapi.yml
  format: yaml
  label: Backrow Recordings API
  slug: backrow-ai-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-recordings-api-openapi.yml
- filename: backrow-ai-tools-api-openapi.yml
  format: yaml
  label: Backrow Tools API
  slug: backrow-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-tools-api-openapi.yml
- filename: backrow-ai-webhooks-api-openapi.yml
  format: yaml
  label: Backrow Webhooks API
  slug: backrow-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: backrow.ai
  spf: true
hosts:
- cert_expires: Jan 20 01:48:57 2027 GMT
  host: backrow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backrow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Backrow
provider_slug: backrow-ai
slug: backrow-ai-domain-security
source_filename: backrow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 01:48:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: backrow.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/backrow-ai/security/backrow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Productivity
- Education
- Knowledge Management
- Software-as-a-Service
---
