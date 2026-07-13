---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carters.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.carters.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: developer.carters.com
  https: false
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.carters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carter''s, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carter's
provider_slug: carter
slug: carter-domain-security
source_filename: carter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.carters.com\n  https: false\n- host: api.carters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: carters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carter/refs/heads/main/security/carter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Children
- Apparel
- Fortune 1000
---
