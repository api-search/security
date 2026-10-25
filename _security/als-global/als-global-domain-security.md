---
api_specs:
- filename: als-global-preference-api-openapi.yml
  format: yaml
  label: ALS Preference API
  slug: als-global-preference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-preference-api-openapi.yml
- filename: als-global-sample-api-openapi.yml
  format: yaml
  label: ALS Sample API
  slug: als-global-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-sample-api-openapi.yml
- filename: als-global-search-api-openapi.yml
  format: yaml
  label: ALS Search API
  slug: als-global-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alsglobal.com
  spf: true
hosts:
- cert_expires: Dec 28 19:42:29 2026 GMT
  host: alsglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Als Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ALS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ALS
provider_slug: als-global
slug: als-global-domain-security
source_filename: als-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alsglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 19:42:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alsglobal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/security/als-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Laboratory Testing
- Environmental Testing
- Inspection
- Certification
- Geochemistry
- Food Testing
- LIMS Integration
---
