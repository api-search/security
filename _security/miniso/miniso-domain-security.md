---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: miniso.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.miniso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miniso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miniso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Miniso
provider_slug: miniso
slug: miniso-domain-security
source_filename: miniso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.miniso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: miniso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miniso/refs/heads/main/security/miniso-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Lifestyle
- Consumer Goods
- Variety Store
- E-commerce
- Merchandise
---
