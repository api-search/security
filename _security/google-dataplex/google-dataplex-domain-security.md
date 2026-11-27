---
api_specs:
- filename: google-dataplex-projects-api-openapi.yml
  format: yaml
  label: Google Dataplex Projects API
  slug: google-dataplex-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dataplex/openapi/google-dataplex-projects-api-openapi.yml
- filename: google-dataplex-organizations-api-openapi.yml
  format: yaml
  label: Google Dataplex Dataplex Organizations API
  slug: google-dataplex-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dataplex/openapi/google-dataplex-organizations-api-openapi.yml
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
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:04 2026 GMT
  host: packages.cloud.google.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: dataplex.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Dataplex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Dataplex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Dataplex
provider_slug: google-dataplex
slug: google-dataplex-domain-security
source_filename: google-dataplex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: packages.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:04 2026 GMT\n  hsts: null\n- host: dataplex.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-dataplex/security/google-dataplex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Governance
- Metadata Management
- Google Cloud
- AI Agents
---
