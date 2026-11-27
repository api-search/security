---
api_specs:
- filename: limitguard-ai-entity-api-openapi.yml
  format: yaml
  label: Limitguard Entity API
  slug: limitguard-ai-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limitguard-ai/openapi/limitguard-ai-entity-api-openapi.yml
- filename: limitguard-ai-risk-api-openapi.yml
  format: yaml
  label: Limitguard Risk API
  slug: limitguard-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limitguard-ai/openapi/limitguard-ai-risk-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:compliance@limitguard.ai"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: limitguard.ai
  spf: true
hosts:
- cert_expires: Feb  6 12:36:08 2027 GMT
  host: limitguard.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Limitguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limitguard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Limitguard
provider_slug: limitguard-ai
slug: limitguard-ai-domain-security
source_filename: limitguard-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: limitguard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 12:36:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: limitguard.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:compliance@limitguard.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/limitguard-ai/security/limitguard-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Lead Validation
- Data Verification
- Software-as-a-Service
- Europe
---
