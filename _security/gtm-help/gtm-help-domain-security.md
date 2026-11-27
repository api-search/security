---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gtm.help
  spf: true
hosts:
- cert_expires: Dec 27 23:45:15 2026 GMT
  host: gtm.help
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gtm.help Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gtm.help, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: gtm.help
provider_slug: gtm-help
slug: gtm-help-domain-security
source_filename: gtm-help-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gtm.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:45:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gtm.help\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gtm-help/security/gtm-help-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Growth
- Software-as-a-Service
- Startups
---
