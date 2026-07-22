---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssladmin.microsoft.com"
  - 0 issue "digicert.com"
  - 0 issue "microsoft.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quad.com
  spf: true
hosts:
- cert_expires: Sep  5 11:28:52 2026 GMT
  host: www.quad.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quad Graphics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quad/Graphics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quad/Graphics
provider_slug: quad-graphics
slug: quad-graphics-domain-security
source_filename: quad-graphics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:28:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quad.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssladmin.microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quad-graphics/refs/heads/main/security/quad-graphics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Print
- Media
---
