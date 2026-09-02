---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carrd.co
  spf: true
hosts:
- cert_expires: Oct 12 03:43:53 2026 GMT
  host: carrd.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carrd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carrd
provider_slug: carrd
slug: carrd-domain-security
source_filename: carrd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrd.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:43:53 2026 GMT\n  hsts: false\ndomains:\n- domain: carrd.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrd/refs/heads/main/security/carrd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Website Builder
- No-Code
- Landing Pages
- Web Hosting
- Site Builder
- Forms
- Software-as-a-Service
---
