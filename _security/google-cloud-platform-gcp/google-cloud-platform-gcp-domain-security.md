---
api_specs:
- filename: google-cloud-platform-gcp-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-gcp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/openapi/google-cloud-platform-gcp-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: compute.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Platform Gcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform-gcp
slug: google-cloud-platform-gcp-domain-security
source_filename: google-cloud-platform-gcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compute.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/security/google-cloud-platform-gcp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Computing
- Data Analytics
- IaaS
- Machine Learning
- PaaS
- SaaS
- Serverless
---
