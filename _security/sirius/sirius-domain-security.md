---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: besirius.io
  spf: true
hosts:
- cert_expires: Aug 23 18:34:44 2026 GMT
  host: besirius.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sirius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sirius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sirius
provider_slug: sirius
slug: sirius-domain-security
source_filename: sirius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: besirius.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:34:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: besirius.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirius/refs/heads/main/security/sirius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sustainability
- ESG
- Critical Minerals
- Supply Chain
- Due Diligence
- Compliance
- Mining
- Metals
- Artificial Intelligence
---
