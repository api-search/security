---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toucantoco.com
  spf: true
hosts:
- cert_expires: Oct  7 04:30:15 2026 GMT
  host: toucantoco.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toucantoco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toucan Toco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Toucan Toco
provider_slug: toucantoco
slug: toucantoco-domain-security
source_filename: toucantoco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toucantoco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: toucantoco.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toucantoco/refs/heads/main/security/toucantoco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Data Visualization
- Data Storytelling
- Dashboards
- AI
---
