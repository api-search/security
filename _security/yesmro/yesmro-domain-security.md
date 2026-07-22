---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yesmro.cn
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: yesmro.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yesmro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for yesmro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: yesmro
provider_slug: yesmro
slug: yesmro-domain-security
source_filename: yesmro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yesmro.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yesmro.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yesmro/refs/heads/main/security/yesmro-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- MRO
- Industrial Supply
- E-commerce
- Procurement
- Factory Automation
- Industrial Parts
- B2B
- China
---
