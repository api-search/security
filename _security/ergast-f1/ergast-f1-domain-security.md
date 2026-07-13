---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ergast.com
  spf: false
hosts:
- cert_expires: Sep 13 14:00:15 2026 GMT
  host: ergast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ergast F1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ergast F1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ergast F1
provider_slug: ergast-f1
slug: ergast-f1-domain-security
source_filename: ergast-f1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ergast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:00:15 2026 GMT\n  hsts: null\ndomains:\n- domain: ergast.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ergast-f1/refs/heads/main/security/ergast-f1-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
