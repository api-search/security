---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: midulcehogar.mx
  spf: true
hosts:
- cert_expires: Sep 30 01:09:44 2026 GMT
  host: midulcehogar.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mi Dulce Hogar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mi Dulce Hogar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mi Dulce Hogar
provider_slug: mi-dulce-hogar
slug: mi-dulce-hogar-domain-security
source_filename: mi-dulce-hogar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: midulcehogar.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:09:44 2026 GMT\n  hsts: false\ndomains:\n- domain: midulcehogar.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mi-dulce-hogar/refs/heads/main/security/mi-dulce-hogar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cleaning Services
- Home Services
- Facility Management
- Mexico
- On-Demand Services
- Consumer
---
