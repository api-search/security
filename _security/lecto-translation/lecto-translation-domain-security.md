---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lecto Translation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lecto Translation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lecto Translation
provider_slug: lecto-translation
slug: lecto-translation-domain-security
source_filename: lecto-translation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lecto-translation/refs/heads/main/security/lecto-translation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Text Analysis
- Public APIs
---
