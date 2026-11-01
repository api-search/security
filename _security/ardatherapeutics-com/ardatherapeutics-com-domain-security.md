---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ardatherapeutics.com
  spf: true
hosts:
- cert_expires: Jan 15 11:59:52 2027 GMT
  host: ardatherapeutics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ardatherapeutics Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arda Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Arda Therapeutics
provider_slug: ardatherapeutics-com
slug: ardatherapeutics-com-domain-security
source_filename: ardatherapeutics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ardatherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:59:52 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ardatherapeutics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ardatherapeutics-com/security/ardatherapeutics-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Biotech
- CellTherapy
- Autoimmune
- PrecisionMedicine
---
