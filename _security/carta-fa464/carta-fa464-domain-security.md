---
api_specs:
- filename: carta-fa464-v1alpha1-api-openapi.yml
  format: yaml
  label: Carta Fa464 V1Alpha1 API
  slug: carta-fa464-v1alpha1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carta-fa464/refs/heads/main/openapi/carta-fa464-v1alpha1-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:administrator@carta.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carta.com
  spf: true
hosts:
- cert_expires: Dec 12 09:28:07 2026 GMT
  host: carta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carta Fa464 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carta Fa464, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carta Fa464
provider_slug: carta-fa464
slug: carta-fa464-domain-security
source_filename: carta-fa464-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 09:28:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carta.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:administrator@carta.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carta-fa464/refs/heads/main/security/carta-fa464-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Equity Management
- Fund Administration
- Legal Compliance
- Cap Table
- Valuation
- Private Capital
- CRM Integration
- AI Automation
---
