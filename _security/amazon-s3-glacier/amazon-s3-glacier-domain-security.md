---
api_specs:
- filename: amazon-s3-glacier-vaults-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier Vaults API
  slug: amazon-s3-glacier-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-vaults-api-openapi.yml
- filename: amazon-s3-glacier-access-policy-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Access Policy API
  slug: amazon-s3-glacier-access-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-access-policy-api-openapi.yml
- filename: amazon-s3-glacier-lock-policy-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Lock Policy API
  slug: amazon-s3-glacier-lock-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-lock-policy-api-openapi.yml
- filename: amazon-s3-glacier-multipart-uploads-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Multipart Uploads API
  slug: amazon-s3-glacier-multipart-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-multipart-uploads-api-openapi.yml
- filename: amazon-s3-glacier-notification-configuration-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Notification Configuration API
  slug: amazon-s3-glacier-notification-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-notification-configuration-api-openapi.yml
- filename: amazon-s3-glacier-operations-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Operations API
  slug: amazon-s3-glacier-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-operations-api-openapi.yml
- filename: amazon-s3-glacier-tags-api-openapi.yml
  format: yaml
  label: Amazon S3 Glacier S3 Glacier Tags API
  slug: amazon-s3-glacier-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-s3-glacier/openapi/amazon-s3-glacier-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: console.aws.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: glacier.amazonaws.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon S3 Glacier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon S3 Glacier, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
slug: amazon-s3-glacier-domain-security
source_filename: amazon-s3-glacier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: console.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n- host: glacier.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-s3-glacier/security/amazon-s3-glacier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Archives
- Backup
- Storage
---
