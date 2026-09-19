---
api_specs:
- filename: google-looker-studio-assets-search-api-openapi.yml
  format: yaml
  label: Google Looker Studio Assets:search API
  slug: google-looker-studio-assets-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/openapi/google-looker-studio-assets-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Nov  2 08:39:48 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:39:03 2026 GMT
  host: datastudio.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Google Looker Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Looker Studio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Looker Studio
provider_slug: google-looker-studio
slug: google-looker-studio-domain-security
source_filename: google-looker-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:39:48 2026 GMT\n  hsts: false\n- host: datastudio.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:39:03 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/security/google-looker-studio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
---
