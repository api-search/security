---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opergo.com
  spf: true
hosts:
- cert_expires: May 22 20:18:33 2027 GMT
  host: opergo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OperGo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OperGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OperGo
provider_slug: opergo-com
slug: opergo-com-domain-security
source_filename: opergo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opergo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 22 20:18:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opergo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opergo-com/security/opergo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Custom Parts
- CNC
- 3D Printing
- Injection Molding
---
