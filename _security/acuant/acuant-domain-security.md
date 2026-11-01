---
api_specs:
- filename: acuant-authentication-api-openapi.yml
  format: yaml
  label: Acuant Authentication API
  slug: acuant-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-authentication-api-openapi.yml
- filename: acuant-chip-data-api-openapi.yml
  format: yaml
  label: Acuant Chip Data API
  slug: acuant-chip-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-chip-data-api-openapi.yml
- filename: acuant-document-data-api-openapi.yml
  format: yaml
  label: Acuant Document Data API
  slug: acuant-document-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-document-data-api-openapi.yml
- filename: acuant-document-instances-api-openapi.yml
  format: yaml
  label: Acuant Document Instances API
  slug: acuant-document-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-document-instances-api-openapi.yml
- filename: acuant-images-api-openapi.yml
  format: yaml
  label: Acuant Images API
  slug: acuant-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-images-api-openapi.yml
- filename: acuant-liveness-api-openapi.yml
  format: yaml
  label: Acuant Liveness API
  slug: acuant-liveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-liveness-api-openapi.yml
- filename: acuant-metadata-api-openapi.yml
  format: yaml
  label: Acuant Metadata API
  slug: acuant-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-metadata-api-openapi.yml
- filename: acuant-operations-for-checking-the-status-of-the-service-api-openapi.yml
  format: yaml
  label: Acuant Operations for Checking the Status of the Service API
  slug: acuant-operations-for-checking-the-status-of-the-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-operations-for-checking-the-status-of-the-service-api-openapi.yml
- filename: acuant-operations-for-facial-matching-api-openapi.yml
  format: yaml
  label: Acuant Operations for Facial Matching API
  slug: acuant-operations-for-facial-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-operations-for-facial-matching-api-openapi.yml
- filename: acuant-health-check-api-openapi.yml
  format: yaml
  label: Acuant Health Check API
  slug: acuant-health-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuant/openapi/acuant-health-check-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuant.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assureid.net
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.acuant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: services.assureid.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: frm.acuant.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acuant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acuant, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acuant
provider_slug: acuant
slug: acuant-domain-security
source_filename: acuant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acuant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.assureid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: frm.acuant.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: acuant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: assureid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/acuant/security/acuant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Document Authentication
- Biometrics
- Face Matching
- Liveness Detection
- KYC
- AML
- ID Capture
---
