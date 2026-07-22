---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fidocure.com
  spf: true
hosts:
- cert_expires: Sep 25 06:34:07 2026 GMT
  host: fidocure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:23:58 2026 GMT
  host: dvm.fidocure.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onehealthcompany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneHealthCompany, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OneHealthCompany
provider_slug: onehealthcompany
slug: onehealthcompany-domain-security
source_filename: onehealthcompany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fidocure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:34:07 2026 GMT\n  hsts: false\n- host: dvm.fidocure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:23:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fidocure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onehealthcompany/refs/heads/main/security/onehealthcompany-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Veterinary
- Animal Health
- Healthcare
- Precision Medicine
- Oncology
- Genomics
- Artificial Intelligence
- Real World Evidence
---
