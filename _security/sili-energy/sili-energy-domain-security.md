---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: silienergy.kr
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: silienergy.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sili Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SILI ENERGY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SILI ENERGY
provider_slug: sili-energy
slug: sili-energy-domain-security
source_filename: sili-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silienergy.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: silienergy.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sili-energy/refs/heads/main/security/sili-energy-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
