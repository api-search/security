---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adm.cc
  spf: true
hosts:
- cert_expires: Dec 18 15:08:19 2026 GMT
  host: adm.cc
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adm Cc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ADM
provider_slug: adm-cc
slug: adm-cc-domain-security
source_filename: adm-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adm.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 15:08:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: adm.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adm-cc/refs/heads/main/security/adm-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Google-Ads
- MCP
---
