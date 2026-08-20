---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backstory.ai
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: people.ai
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.backstory.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: mcp.people.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backstory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backstory, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Backstory
provider_slug: backstory
slug: backstory-domain-security
source_filename: backstory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backstory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.people.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: backstory.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: people.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstory/refs/heads/main/security/backstory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Revenue Intelligence
- Sales
- CRM
- Sales Analytics
- Forecasting
- Revenue Operations
- MCP
- AI Agents
---
