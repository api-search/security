---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brandize.me
  spf: false
hosts:
- cert_expires: Jan  6 08:36:08 2027 GMT
  host: brandize.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brandize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Brandize
provider_slug: brandize-me
slug: brandize-me-domain-security
source_filename: brandize-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandize.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:36:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brandize.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/brandize-me/security/brandize-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Logo
- Design
- Branding
- Software-as-a-Service
- Company
---
