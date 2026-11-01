---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sdworx.com
  spf: true
hosts:
- cert_expires: Dec 28 08:35:03 2026 GMT
  host: sdworx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sd Worx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SD Worx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SD Worx
provider_slug: sd-worx
slug: sd-worx-domain-security
source_filename: sd-worx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sdworx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 08:35:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sdworx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sd-worx/security/sd-worx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- Payroll
- Workforce-Management
- Europe
- Cloud
---
