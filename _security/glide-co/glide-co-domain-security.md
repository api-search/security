---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glide.co
  spf: true
hosts:
- cert_expires: Dec 20 05:41:09 2026 GMT
  host: glide.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Glide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Glide
provider_slug: glide-co
slug: glide-co-domain-security
source_filename: glide-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glide.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 05:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: glide.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/glide-co/security/glide-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Banking
- Payments
- Global
---
