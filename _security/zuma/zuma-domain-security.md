---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getzuma.com
  spf: true
hosts:
- cert_expires: Sep 29 05:12:06 2026 GMT
  host: www.getzuma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zuma
provider_slug: zuma
slug: zuma-domain-security
source_filename: zuma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getzuma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:12:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getzuma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuma/refs/heads/main/security/zuma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Multifamily
- Property Management
- Artificial Intelligence
- Leasing
- Rent Collections
- Conversational AI
---
