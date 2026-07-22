---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leta.ai
  spf: true
hosts:
- cert_expires: Aug 29 05:15:44 2026 GMT
  host: leta.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:20:36 2026 GMT
  host: api.leta.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 14:06:24 2026 GMT
  host: cloud.leta.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Leta
provider_slug: leta
slug: leta-domain-security
source_filename: leta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:15:44 2026 GMT\n  hsts: false\n- host: api.leta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:20:36 2026 GMT\n  hsts: false\n- host: cloud.leta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:06:24 2026 GMT\n  hsts: false\ndomains:\n- domain: leta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leta/refs/heads/main/security/leta-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Logistics
- Delivery
- Last Mile Delivery
- Supply Chain
- Route Optimization
- Fleet Management
- Transportation
- Artificial Intelligence
- Africa
- SaaS
---
