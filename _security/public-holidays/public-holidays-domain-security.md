---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abstractapi.com
  spf: false
hosts:
- cert_expires: Sep 10 07:12:58 2026 GMT
  host: www.abstractapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Public Holidays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Public Holidays, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Public Holidays
provider_slug: public-holidays
slug: public-holidays-domain-security
source_filename: public-holidays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abstractapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:12:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abstractapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public-holidays/refs/heads/main/security/public-holidays-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Public APIs
---
