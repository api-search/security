---
api_specs:
- filename: v7-labs-annotations-api-openapi.yml
  format: yaml
  label: V7 Annotations API
  slug: v7-labs-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-annotations-api-openapi.yml
- filename: v7-labs-classes-api-openapi.yml
  format: yaml
  label: V7 Classes API
  slug: v7-labs-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-classes-api-openapi.yml
- filename: v7-labs-datasets-api-openapi.yml
  format: yaml
  label: V7 Datasets API
  slug: v7-labs-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-datasets-api-openapi.yml
- filename: v7-labs-exports-api-openapi.yml
  format: yaml
  label: V7 Exports API
  slug: v7-labs-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-exports-api-openapi.yml
- filename: v7-labs-items-api-openapi.yml
  format: yaml
  label: V7 Items API
  slug: v7-labs-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-items-api-openapi.yml
- filename: v7-labs-workflows-api-openapi.yml
  format: yaml
  label: V7 Workflows API
  slug: v7-labs-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: v7labs.com
  spf: true
hosts:
- cert_expires: Sep  7 15:01:47 2026 GMT
  host: www.v7labs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 11:30:09 2026 GMT
  host: docs.v7labs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: darwin.v7labs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: V7 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for V7, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: V7
provider_slug: v7-labs
slug: v7-labs-domain-security
source_filename: v7-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.v7labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.v7labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:30:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: darwin.v7labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: v7labs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/security/v7-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Training Data
- Data Labeling
- Annotation
- Document AI
- Computer Vision
---
