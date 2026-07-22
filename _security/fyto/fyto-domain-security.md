---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fyto.us
  spf: false
hosts:
- cert_expires: Sep  6 18:46:47 2026 GMT
  host: fyto.us
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fyto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fyto
provider_slug: fyto
slug: fyto-domain-security
source_filename: fyto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fyto.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:46:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: fyto.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyto/refs/heads/main/security/fyto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Agriculture
- AgTech
- Robotics
- Sustainability
- Cleantech
- Animal Feed
- Dairy
---
