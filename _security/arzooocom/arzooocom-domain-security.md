---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arzooo.com
  spf: true
hosts:
- cert_expires: Dec  3 03:38:16 2026 GMT
  host: www.arzooo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arzooocom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arzooocom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arzooocom
provider_slug: arzooocom
slug: arzooocom-domain-security
source_filename: arzooocom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arzooo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 03:38:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arzooo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arzooocom/refs/heads/main/security/arzooocom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Retail
- India
- E-Commerce
---
