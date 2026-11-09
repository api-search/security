---
api_specs:
- filename: gcp-cloud-storage-bucketaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage BucketAccessControls API
  slug: gcp-cloud-storage-bucketaccesscontrols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-bucketaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Buckets API
  slug: gcp-cloud-storage-buckets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-buckets-api-openapi.yml
- filename: gcp-cloud-storage-defaultobjectaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage DefaultObjectAccessControls API
  slug: gcp-cloud-storage-defaultobjectaccesscontrols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-defaultobjectaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-objectaccesscontrols-api-openapi.yml
  format: yaml
  label: Google Cloud Storage ObjectAccessControls API
  slug: gcp-cloud-storage-objectaccesscontrols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-objectaccesscontrols-api-openapi.yml
- filename: gcp-cloud-storage-objects-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Objects API
  slug: gcp-cloud-storage-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-objects-api-openapi.yml
- filename: gcp-cloud-storage-anywherecaches-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Anywhere Caches API
  slug: gcp-cloud-storage-anywherecaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-anywherecaches-api-openapi.yml
- filename: gcp-cloud-storage-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Folders API
  slug: gcp-cloud-storage-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-folders-api-openapi.yml
- filename: gcp-cloud-storage-managedfolders-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Managed Folders API
  slug: gcp-cloud-storage-managedfolders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-managedfolders-api-openapi.yml
- filename: gcp-cloud-storage-notifications-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Notifications API
  slug: gcp-cloud-storage-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-notifications-api-openapi.yml
- filename: gcp-cloud-storage-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Operations API
  slug: gcp-cloud-storage-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-operations-api-openapi.yml
- filename: gcp-cloud-storage-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Projects API
  slug: gcp-cloud-storage-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-projects-api-openapi.yml
- filename: gcp-cloud-storage-rapidcaches-api-openapi.yml
  format: yaml
  label: Google Cloud Storage Rapid Caches API
  slug: gcp-cloud-storage-rapidcaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gcp-cloud-storage/openapi/gcp-cloud-storage-rapidcaches-api-openapi.yml
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
- cert_expires: Dec 30 19:11:54 2026 GMT
  host: storage.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gcp Cloud Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Storage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
slug: gcp-cloud-storage-domain-security
source_filename: gcp-cloud-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: storage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:11:54 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gcp-cloud-storage/security/gcp-cloud-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
---
