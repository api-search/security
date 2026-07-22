---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hollyfrontier.com
  spf: true
hosts:
- cert_expires: Aug 27 20:50:00 2026 GMT
  host: www.hollyfrontier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hollyfrontier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hollyfrontier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: hollyfrontier
provider_slug: hollyfrontier
slug: hollyfrontier-domain-security
source_filename: hollyfrontier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hollyfrontier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hollyfrontier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hollyfrontier/refs/heads/main/security/hollyfrontier-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fortune 500
---
