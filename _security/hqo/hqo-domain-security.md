---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hqo.com
  spf: true
hosts:
- cert_expires: Sep 16 16:51:56 2026 GMT
  host: www.hqo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HqO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HqO
provider_slug: hqo
slug: hqo-domain-security
source_filename: hqo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hqo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:51:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hqo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hqo/refs/heads/main/security/hqo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Commercial Real Estate
- Workplace Experience
- Tenant Experience
- Real Estate Technology
- Building Management
- Property Management
---
