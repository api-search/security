---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goji.agency
  spf: true
hosts:
- cert_expires: Dec 30 04:13:54 2026 GMT
  host: goji.agency
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GOJI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GOJI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GOJI
provider_slug: goji-agency
slug: goji-agency-domain-security
source_filename: goji-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goji.agency\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 04:13:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goji.agency\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goji-agency/security/goji-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Agency
- SEO
- Branding
- Artificial Intelligence
- Web Development
---
