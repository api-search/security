---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alba-app.com
  spf: false
hosts:
- cert_expires: Nov  7 21:07:08 2026 GMT
  host: alba-app.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alba, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Alba
provider_slug: alba
slug: alba-domain-security
source_filename: alba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alba-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 21:07:08 2026 GMT\n  hsts: false\ndomains:\n- domain: alba-app.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alba/refs/heads/main/security/alba-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
