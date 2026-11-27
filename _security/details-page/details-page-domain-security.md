---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: details.page
  spf: true
hosts:
- cert_expires: Dec 11 09:26:01 2026 GMT
  host: details.page
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: details.page Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for details.page, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: details.page
provider_slug: details-page
slug: details-page-domain-security
source_filename: details-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: details.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 09:26:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: details.page\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/details-page/security/details-page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Platform
- Event Management
- Aggregator
- RSVP
- Free
---
