---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eliq.com
  spf: true
hosts:
- cert_expires: Sep 26 17:05:18 2026 GMT
  host: eliq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:42:32 2026 GMT
  host: developer.eliq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eliq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eliq, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eliq
provider_slug: eliq
slug: eliq-domain-security
source_filename: eliq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.eliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:42:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/security/eliq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Analytics
- Sustainability
---
