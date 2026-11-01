---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: attestvio.com
  spf: true
hosts:
- cert_expires: Dec  3 15:26:45 2026 GMT
  host: attestvio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attestvio Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for attestvio-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: attestvio-com
provider_slug: attestvio-com
slug: attestvio-com-domain-security
source_filename: attestvio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attestvio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 15:26:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: attestvio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/attestvio-com/security/attestvio-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- HR
- Compliance
- SaaS
- Software
- API
---
