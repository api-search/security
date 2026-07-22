---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inato.com
  spf: true
hosts:
- cert_expires: Oct  3 08:18:50 2026 GMT
  host: inato.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inato
provider_slug: inato
slug: inato-domain-security
source_filename: inato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inato/refs/heads/main/security/inato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- Pharmaceuticals
- Clinical Research
- Marketplace
- Artificial Intelligence
---
