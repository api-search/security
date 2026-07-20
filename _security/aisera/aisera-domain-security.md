---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aisera.com
  spf: true
hosts:
- cert_expires: Oct  2 01:03:44 2026 GMT
  host: aisera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aisera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aisera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aisera
provider_slug: aisera
slug: aisera-domain-security
source_filename: aisera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aisera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aisera.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisera/refs/heads/main/security/aisera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agentic AI
- Conversational AI
- IT Service Management
- Customer Service
- Enterprise Search
- AI Copilot
- Knowledge Management
- Workflow Automation
- Large Language Models
---
