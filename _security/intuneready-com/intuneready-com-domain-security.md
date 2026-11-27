---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intuneready.com
  spf: true
hosts:
- cert_expires: Dec 13 17:14:09 2026 GMT
  host: intuneready.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intune Ready Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intune Ready, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Intune Ready
provider_slug: intuneready-com
slug: intuneready-com-domain-security
source_filename: intuneready-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intuneready.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 17:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intuneready.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/intuneready-com/security/intuneready-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Microsoft
- Intune
- IT Services
- Small Business
---
