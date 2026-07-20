---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ajar.com.kw
  spf: true
hosts:
- cert_expires: Sep  8 12:35:07 2026 GMT
  host: ajar.com.kw
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ajar Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ajar Online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ajar Online
provider_slug: ajar-online
slug: ajar-online-domain-security
source_filename: ajar-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ajar.com.kw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:35:07 2026 GMT\n  hsts: null\ndomains:\n- domain: ajar.com.kw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajar-online/refs/heads/main/security/ajar-online-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Property Management
- Rent Payments
- Payments
- Kuwait
- MENA
---
