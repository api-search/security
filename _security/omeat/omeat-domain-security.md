---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evergreen.food
  spf: true
hosts:
- cert_expires: Aug 28 23:14:06 2026 GMT
  host: www.evergreen.food
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omeat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omeat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Omeat
provider_slug: omeat
slug: omeat-domain-security
source_filename: omeat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evergreen.food\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evergreen.food\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omeat/refs/heads/main/security/omeat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Cultivated Meat
- Food Technology
- Biotechnology
- Agriculture
- Sustainability
---
