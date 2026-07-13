---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tattleapp.com
  spf: false
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: get.tattleapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tattle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tattle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tattle
provider_slug: tattle
slug: tattle-domain-security
source_filename: tattle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get.tattleapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tattleapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tattle/refs/heads/main/security/tattle-domain-security.yml
summary_line: TLSv1.3
tags:
- Restaurant
- Guest Feedback
- Customer Experience
- Review Management
- Analytics
- Integrations
---
