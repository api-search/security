---
api_specs:
- filename: kameleoon-openapi.yml
  format: yaml
  label: Kameleoon Automation API
  slug: kameleoon-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/openapi/kameleoon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kameleoon.com
  spf: true
hosts:
- cert_expires: Aug 17 11:53:12 2026 GMT
  host: www.kameleoon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 13:16:41 2026 GMT
  host: developers.kameleoon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 08:05:21 2026 GMT
  host: api.kameleoon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kameleoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kameleoon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kameleoon
provider_slug: kameleoon
slug: kameleoon-domain-security
source_filename: kameleoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kameleoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:53:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.kameleoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 13:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kameleoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:05:21 2026 GMT\n  hsts: null\ndomains:\n- domain: kameleoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/security/kameleoon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Experimentation
- AB Testing
- Personalization
- Feature Flags
- AI
---
