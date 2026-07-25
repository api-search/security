---
api_specs:
- filename: amazon-opensearch-domain-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Domain API
  slug: amazon-opensearch-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-domain-api-openapi.yml
- filename: amazon-opensearch-es-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Es API
  slug: amazon-opensearch-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-es-api-openapi.yml
- filename: amazon-opensearch-packages-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Packages API
  slug: amazon-opensearch-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-packages-api-openapi.yml
- filename: amazon-opensearch-tags-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Tags API
  slug: amazon-opensearch-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-tags-api-openapi.yml
- filename: amazon-opensearch-tags-removal-api-openapi.yml
  format: yaml
  label: Amazon OpenSearch Service API Tags Removal API
  slug: amazon-opensearch-tags-removal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/openapi/amazon-opensearch-tags-removal-api-openapi.yml
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
- host: es.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Opensearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon OpenSearch Service API, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
slug: amazon-opensearch-domain-security
source_filename: amazon-opensearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: es.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/security/amazon-opensearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Elasticsearch
- Search
---
