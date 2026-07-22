---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glg.com
  spf: true
hosts:
- cert_expires: Sep 20 19:38:45 2026 GMT
  host: glg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gerson Lehrman Group Glg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gerson Lehrman Group (GLG), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gerson Lehrman Group (GLG)
provider_slug: gerson-lehrman-group-glg
slug: gerson-lehrman-group-glg-domain-security
source_filename: gerson-lehrman-group-glg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:38:45 2026 GMT\n  hsts: false\ndomains:\n- domain: glg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gerson-lehrman-group-glg/refs/heads/main/security/gerson-lehrman-group-glg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Expert Network
- Market Research
- Insights
- Consulting
- Professional Services
- Advisory
---
