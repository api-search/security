---
api_specs:
- filename: pexels-openapi.yml
  format: yaml
  label: Pexels API
  slug: pexels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexels/refs/heads/main/openapi/pexels-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pexels.com
  spf: true
hosts:
- cert_expires: Sep  4 15:38:41 2026 GMT
  host: www.pexels.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 11:17:20 2026 GMT
  host: api.pexels.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pexels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pexels, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pexels
provider_slug: pexels
slug: pexels-domain-security
source_filename: pexels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pexels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:38:41 2026 GMT\n  hsts: null\n- host: api.pexels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:17:20 2026 GMT\n  hsts: false\ndomains:\n- domain: pexels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexels/refs/heads/main/security/pexels-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Photos
- Stock Media
- Videos
---
