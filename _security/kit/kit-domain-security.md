---
api_specs:
- filename: kit-openapi.yml
  format: yaml
  label: Kit API V4
  slug: kit-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/openapi/kit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kit.com
  spf: true
hosts:
- cert_expires: Sep 21 16:51:44 2026 GMT
  host: kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 14:29:40 2026 GMT
  host: developers.kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kit
provider_slug: kit
slug: kit-domain-security
source_filename: kit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:51:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.kit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/security/kit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Creator Economy
- Newsletters
- Automation
- Subscribers
---
