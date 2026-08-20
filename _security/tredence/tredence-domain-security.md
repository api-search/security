---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tredence.com
  spf: true
hosts:
- cert_expires: Nov  3 08:40:56 2026 GMT
  host: www.tredence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tredence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tredence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tredence
provider_slug: tredence
slug: tredence-domain-security
source_filename: tredence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tredence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 08:40:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tredence.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tredence/refs/heads/main/security/tredence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Science
- Artificial Intelligence
- Analytics
- Machine-Learning
- Consulting
- Data Engineering
- MLOps
- Agentic AI
- Supply Chain
---
