---
api_specs:
- filename: brandlive-brandlive-api-api-openapi.yml
  format: yaml
  label: Brandlive Brandlive API
  slug: brandlive-brandlive-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/openapi/brandlive-brandlive-api-api-openapi.yml
- filename: brandlive-event-api-openapi.yml
  format: yaml
  label: Brandlive Event API
  slug: brandlive-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/openapi/brandlive-event-api-openapi.yml
- filename: brandlive-registration-api-openapi.yml
  format: yaml
  label: Brandlive Registration API
  slug: brandlive-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/openapi/brandlive-registration-api-openapi.yml
- filename: brandlive-registration-code-check-api-openapi.yml
  format: yaml
  label: Brandlive Registration Code Check API
  slug: brandlive-registration-code-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/openapi/brandlive-registration-code-check-api-openapi.yml
- filename: brandlive-template-api-openapi.yml
  format: yaml
  label: Brandlive Template API
  slug: brandlive-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/openapi/brandlive-template-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandlive.com
  spf: true
hosts:
- cert_expires: Dec 29 15:06:37 2026 GMT
  host: www.brandlive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brandlive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandlive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandlive
provider_slug: brandlive
slug: brandlive-domain-security
source_filename: brandlive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandlive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brandlive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandlive/refs/heads/main/security/brandlive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Streaming
- Live Events
- Enterprise
---
