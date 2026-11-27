---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: natgaslens.com
  spf: false
hosts:
- cert_expires: Jan 18 13:12:42 2027 GMT
  host: natgaslens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NatGasLens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NatGasLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NatGasLens
provider_slug: natgaslens-com
slug: natgaslens-com-domain-security
source_filename: natgaslens-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: natgaslens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 13:12:42 2027 GMT\n  hsts: false\ndomains:\n- domain: natgaslens.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/natgaslens-com/security/natgaslens-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Data
- Natural Gas
- Monitoring
---
