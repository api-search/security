---
api_specs:
- filename: jotform-openapi.yml
  format: yaml
  label: Jotform REST API (Standard / US)
  slug: rest-us
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jotform.com
  spf: true
hosts:
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: www.jotform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: api.jotform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: eu-api.jotform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jotform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jotform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jotform
provider_slug: jotform
slug: jotform-domain-security
source_filename: jotform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jotform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jotform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\n- host: eu-api.jotform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jotform.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/security/jotform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forms
- Surveys
- No-Code
- Data Collection
- Workflow
- HIPAA
- EU
---
