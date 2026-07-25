---
api_specs:
- filename: huma-platform-openapi-original.yml
  format: yaml
  label: Huma Integration API
  slug: huma-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/openapi/huma-platform-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huma.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: huma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 17:54:29 2026 GMT
  host: docs.huma.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: workspace-gcp-uk.api.huma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Huma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huma
provider_slug: huma
slug: huma-domain-security
source_filename: huma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.huma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: workspace-gcp-uk.api.huma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: huma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/security/huma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United Kingdom
- Remote Patient Monitoring
- Telehealth
- Digital Health
- Clinical Trials
- SDK
- Medical Device Software
- Population Health
---
