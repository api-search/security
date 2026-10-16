---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carsonlife.com
  spf: true
hosts:
- cert_expires: Dec 31 15:18:02 2026 GMT
  host: en.carsonlife.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carson Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carson Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carson Life
provider_slug: carson-life
slug: carson-life-domain-security
source_filename: carson-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.carsonlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 15:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: carsonlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carson-life/refs/heads/main/security/carson-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Beauty
- E‑commerce
- Skincare
- Weight‑loss
- Vitamins
---
