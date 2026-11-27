---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heydolfin.com
  spf: true
hosts:
- cert_expires: Feb  6 21:32:31 2027 GMT
  host: heydolfin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dolfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dolfin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dolfin
provider_slug: heydolfin-com
slug: heydolfin-com-domain-security
source_filename: heydolfin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heydolfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 21:32:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heydolfin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heydolfin-com/security/heydolfin-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- Artificial Intelligence
- Commissions
- Revenue Operations
- Finance
---
