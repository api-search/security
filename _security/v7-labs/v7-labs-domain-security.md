---
api_specs:
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Items & Upload API
  slug: items-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Workflows & Stages API
  slug: workflows-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotation Classes API
  slug: classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Exports API
  slug: exports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
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
