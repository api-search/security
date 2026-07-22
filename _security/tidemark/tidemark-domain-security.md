---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tidemark.com
  spf: true
hosts:
- cert_expires: Oct 11 07:04:45 2026 GMT
  host: www.tidemark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidemark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidemark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tidemark
provider_slug: tidemark
slug: tidemark-domain-security
source_filename: tidemark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tidemark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:04:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tidemark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidemark/refs/heads/main/security/tidemark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Performance Management
- Financial Planning
- Budgeting and Forecasting
- Analytics
- Planning Software
- a16z Portfolio
---
