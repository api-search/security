---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digimarc.com
  spf: true
hosts:
- cert_expires: Dec  2 02:08:19 2026 GMT
  host: www.digimarc.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digimarc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digimarc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digimarc
provider_slug: digimarc
slug: digimarc-domain-security
source_filename: digimarc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digimarc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 02:08:19 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: digimarc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/digimarc/security/digimarc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Digital Watermarking
- Product Authentication
- Anti-Counterfeiting
- Connected Packaging
- QR Codes
- Content Provenance
- Mobile SDK
---
