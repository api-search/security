---
api_specs:
- filename: google-cloud-kms-folders-api-openapi.yml
  format: yaml
  label: Google Cloud KMS Folders API
  slug: google-cloud-kms-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-kms/openapi/google-cloud-kms-folders-api-openapi.yml
- filename: google-cloud-kms-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud KMS Organizations API
  slug: google-cloud-kms-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-kms/openapi/google-cloud-kms-organizations-api-openapi.yml
- filename: google-cloud-kms-projects-api-openapi.yml
  format: yaml
  label: Google Cloud KMS Projects API
  slug: google-cloud-kms-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-kms/openapi/google-cloud-kms-projects-api-openapi.yml
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
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: cloudkms.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Cloud KMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud KMS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud KMS
provider_slug: google-cloud-kms
slug: google-cloud-kms-domain-security
source_filename: google-cloud-kms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloudkms.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-kms/security/google-cloud-kms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptography
- Encryption
- Google Cloud
- Key Management
- KMS
- Security
---
