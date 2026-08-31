---
api_specs:
- filename: cloudflare-r2-buckets-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Buckets API
  slug: cloudflare-r2-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-buckets-api-openapi.yml
- filename: cloudflare-r2-cors-api-openapi.yml
  format: yaml
  label: Cloudflare R2 CORS API
  slug: cloudflare-r2-cors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-cors-api-openapi.yml
- filename: cloudflare-r2-credential-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Credential Management API
  slug: cloudflare-r2-credential-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-credential-management-api-openapi.yml
- filename: cloudflare-r2-lifecycle-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Lifecycle API
  slug: cloudflare-r2-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-lifecycle-api-openapi.yml
- filename: cloudflare-r2-maintenance-configuration-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Maintenance Configuration API
  slug: cloudflare-r2-maintenance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-maintenance-configuration-api-openapi.yml
- filename: cloudflare-r2-multipart-upload-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Multipart Upload API
  slug: cloudflare-r2-multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-multipart-upload-api-openapi.yml
- filename: cloudflare-r2-namespace-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Namespace Management API
  slug: cloudflare-r2-namespace-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-namespace-management-api-openapi.yml
- filename: cloudflare-r2-objects-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Objects API
  slug: cloudflare-r2-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-objects-api-openapi.yml
- filename: cloudflare-r2-r2-account-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Account API
  slug: cloudflare-r2-r2-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-account-api-openapi.yml
- filename: cloudflare-r2-r2-bucket-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Bucket API
  slug: cloudflare-r2-r2-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-bucket-api-openapi.yml
- filename: cloudflare-r2-r2-catalog-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Catalog Management API
  slug: cloudflare-r2-r2-catalog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-catalog-management-api-openapi.yml
- filename: cloudflare-r2-r2-object-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Object API
  slug: cloudflare-r2-r2-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-object-api-openapi.yml
- filename: cloudflare-r2-table-maintenance-configuration-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Table Maintenance Configuration API
  slug: cloudflare-r2-table-maintenance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-table-maintenance-configuration-api-openapi.yml
- filename: cloudflare-r2-table-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Table Management API
  slug: cloudflare-r2-table-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-table-management-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:tls-abuse@cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloudflare.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: cloudflarestorage.com
  spf: false
hosts:
- cert_expires: Oct  4 07:46:56 2026 GMT
  host: www.cloudflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:43:14 2026 GMT
  host: developers.cloudflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: <account_id>.r2.cloudflarestorage.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cloudflare R2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudflare R2, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cloudflare R2
provider_slug: cloudflare-r2
slug: cloudflare-r2-domain-security
source_filename: cloudflare-r2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: <account_id>.r2.cloudflarestorage.com\n  https: false\ndomains:\n- domain: cloudflare.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:tls-abuse@cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cloudflarestorage.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/security/cloudflare-r2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Object Storage
- Cloud Storage
- S3-Compatible
- Egress-Free
- Buckets
- Developer Platform
- Cloudflare
---
