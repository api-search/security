---
api_specs:
- filename: crowdin-openapi.yml
  format: yaml
  label: Crowdin REST API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdin/refs/heads/main/openapi/crowdin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crowdin.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: crowdin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 10:04:01 2026 GMT
  host: support.crowdin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.crowdin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crowdin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crowdin
provider_slug: crowdin
slug: crowdin-domain-security
source_filename: crowdin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.crowdin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.crowdin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: crowdin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdin/refs/heads/main/security/crowdin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- Translation
- TMS
- REST
- GraphQL
- Developer Tools
- Enterprise
---
