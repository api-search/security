---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docks.io
  spf: true
hosts:
- cert_expires: Dec 28 03:04:14 2026 GMT
  host: docks.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docks Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e-companion UG (haftungsbeschränkt), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: e-companion UG (haftungsbeschränkt)
provider_slug: docks-io
slug: docks-io-domain-security
source_filename: docks-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 03:04:14 2026 GMT\n  hsts: false\ndomains:\n- domain: docks.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/docks-io/security/docks-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Documentation
- Machinery
- EU-Regulation
- QR Codes
---
