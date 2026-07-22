---
api_specs:
- filename: doc.yaml
  format: yaml
  label: Sigfox Cloud API
  slug: sigfox-cloud-api
  spec_type: OpenAPI
  url: https://api.sigfox.com/v2/doc.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sigfox.com
  spf: true
hosts:
- cert_expires: Sep  8 18:01:25 2026 GMT
  host: sigfox.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 21:38:41 2026 GMT
  host: support.sigfox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.sigfox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sigfox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sigfox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sigfox
provider_slug: sigfox
slug: sigfox-domain-security
source_filename: sigfox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sigfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:01:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: support.sigfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 21:38:41 2026 GMT\n  hsts: false\n- host: api.sigfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sigfox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigfox/refs/heads/main/security/sigfox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Industrial, Energy & Iot
- IoT
- LPWAN
- Connectivity
- Device Management
- Networking
- Telecommunications
---
