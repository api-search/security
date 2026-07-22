---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asetek.com
  spf: true
hosts:
- cert_expires: Aug 24 15:23:49 2026 GMT
  host: www.asetek.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asetek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asetek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Asetek
provider_slug: asetek
slug: asetek-domain-security
source_filename: asetek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asetek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:23:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: asetek.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asetek/refs/heads/main/security/asetek-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Hardware
- Liquid Cooling
- Thermal Management
- Data Center
- High Performance Computing
- Sim Racing
---
