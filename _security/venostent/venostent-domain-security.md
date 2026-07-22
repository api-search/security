---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: venostent.com
  spf: true
hosts:
- cert_expires: Sep 26 17:16:42 2026 GMT
  host: venostent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Venostent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venostent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Venostent
provider_slug: venostent
slug: venostent-domain-security
source_filename: venostent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venostent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:16:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: venostent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venostent/refs/heads/main/security/venostent-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Medical Devices
- MedTech
- Healthcare
- Dialysis
- Vascular Access
- Nephrology
- Bioabsorbable Implants
---
