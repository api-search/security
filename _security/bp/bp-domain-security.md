---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bp.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.bp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: developer.bp.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BP
provider_slug: bp
slug: bp-domain-security
source_filename: bp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: developer.bp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: bp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/security/bp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil
- Gas
- Renewables
- Developer Platform
---
