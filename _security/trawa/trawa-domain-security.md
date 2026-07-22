---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:infosec@trawa.de"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: trawa.de
  spf: true
hosts:
- cert_expires: Oct  3 20:39:02 2026 GMT
  host: www.trawa.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trawa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for trawa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: trawa
provider_slug: trawa
slug: trawa-domain-security
source_filename: trawa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trawa.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trawa.de\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:infosec@trawa.de\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trawa/refs/heads/main/security/trawa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Energy Management
- Electricity
- Renewable Energy
- Sustainability
- Green Energy
- Procurement
- SaaS
- Germany
---
