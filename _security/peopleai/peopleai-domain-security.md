---
description: ''
domains:
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
- cert_expires: Oct  8 13:32:50 2026 GMT
  host: www.people.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peopleai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for People.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: People.ai
provider_slug: peopleai
slug: peopleai-domain-security
source_filename: peopleai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.people.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: people.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleai/refs/heads/main/security/peopleai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Revenue Intelligence
- Sales
- Artificial Intelligence
- CRM
- Sales Automation
- Forecasting
- Enterprise
---
