---
api_specs:
- filename: google-data-studio-api-openapi.yml
  format: yaml
  label: Google Data Studio API
  slug: google-data-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-api-openapi.yml
- filename: google-data-studio-linking-api-openapi.yml
  format: yaml
  label: Looker Studio Linking API
  slug: looker-studio-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-linking-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: lookerstudio.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Data Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Data Studio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Data Studio
provider_slug: google-data-studio
slug: google-data-studio-domain-security
source_filename: google-data-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lookerstudio.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/security/google-data-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
---
