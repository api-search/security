---
api_specs:
- filename: google-cloud-spanner-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Spanner Cloud Spanner Projects API
  slug: google-cloud-spanner-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-spanner/openapi/google-cloud-spanner-projects-api-openapi.yml
- filename: google-cloud-spanner-scans-api-openapi.yml
  format: yaml
  label: Google Cloud Spanner Cloud Spanner Scans API
  slug: google-cloud-spanner-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-spanner/openapi/google-cloud-spanner-scans-api-openapi.yml
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
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:11:53 2026 GMT
  host: spanner.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Cloud Spanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Spanner, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Spanner
provider_slug: google-cloud-spanner
slug: google-cloud-spanner-domain-security
source_filename: google-cloud-spanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spanner.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:11:53 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-spanner/security/google-cloud-spanner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Distributed
- Google Cloud
- Relational
- SQL
---
