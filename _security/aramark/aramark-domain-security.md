---
api_specs:
- filename: marko-api.yml
  format: yaml
  label: Aramark Marko API
  slug: marko-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/marko-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aramark.net
  spf: true
hosts:
- cert_expires: Aug 23 19:52:25 2026 GMT
  host: marko-developers.aramark.net
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: www.marko.aramark.net
  https: false
kind: domain-security
layout: security
method: probed
name: Aramark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aramark, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aramark
provider_slug: aramark
slug: aramark-domain-security
source_filename: aramark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marko-developers.aramark.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:52:25 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.marko.aramark.net\n  https: false\ndomains:\n- domain: aramark.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/security/aramark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
---
