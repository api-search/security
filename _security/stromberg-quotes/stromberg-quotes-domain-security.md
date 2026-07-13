---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stromberg-api.de
  spf: true
hosts:
- cert_expires: Aug 10 20:16:55 2026 GMT
  host: www.stromberg-api.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stromberg Quotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stromberg Quotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stromberg Quotes
provider_slug: stromberg-quotes
slug: stromberg-quotes-domain-security
source_filename: stromberg-quotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stromberg-api.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 20:16:55 2026 GMT\n  hsts: false\ndomains:\n- domain: stromberg-api.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stromberg-quotes/refs/heads/main/security/stromberg-quotes-domain-security.yml
summary_line: TLSv1.3
tags:
- Video
- Public APIs
---
