---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tapestry.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.tapestry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.tapestry.com
  https: false
- host: api.tapestry.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tapestry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tapestry, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tapestry
provider_slug: tapestry
slug: tapestry-domain-security
source_filename: tapestry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tapestry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tapestry.com\n  https: false\n- host: api.tapestry.com\n  https: false\ndomains:\n- domain: tapestry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapestry/refs/heads/main/security/tapestry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Luxury
- Fashion
---
