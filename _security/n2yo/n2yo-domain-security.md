---
api_specs:
- filename: n2yo-openapi.yml
  format: yaml
  label: N2YO.com API
  slug: n2yo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n2yo/main/openapi/n2yo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: n2yo.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.n2yo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug  4 16:53:01 2026 GMT
  host: api.n2yo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N2Yo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for N2YO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: N2YO
provider_slug: n2yo
slug: n2yo-domain-security
source_filename: n2yo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.n2yo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.n2yo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 16:53:01 2026 GMT\n  hsts: false\ndomains:\n- domain: n2yo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n2yo/refs/heads/main/security/n2yo-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Satellites
- Space
- Tracking
---
