---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: korushield.com
  spf: true
hosts:
- cert_expires: Dec 26 22:09:08 2026 GMT
  host: korushield.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Koru Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koru Shield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koru Shield
provider_slug: korushield-com
slug: korushield-com-domain-security
source_filename: korushield-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: korushield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 22:09:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: korushield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/korushield-com/security/korushield-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- Security
- Privacy
- Advertising
- Family-safe
- Company
---
