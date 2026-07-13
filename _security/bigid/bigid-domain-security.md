---
api_specs:
- filename: bigid-authentication-api-openapi.yml
  format: yaml
  label: BigID Authentication API
  slug: bigid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-authentication-api-openapi.yml
- filename: bigid-data-sources-api-openapi.yml
  format: yaml
  label: BigID Data Sources API
  slug: bigid-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-sources-api-openapi.yml
- filename: bigid-scans-api-openapi.yml
  format: yaml
  label: BigID Scans API
  slug: bigid-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-scans-api-openapi.yml
- filename: bigid-data-catalog-api-openapi.yml
  format: yaml
  label: BigID Data Catalog API
  slug: bigid-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-catalog-api-openapi.yml
- filename: bigid-cluster-analysis-api-openapi.yml
  format: yaml
  label: BigID Cluster Analysis API
  slug: bigid-cluster-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-cluster-analysis-api-openapi.yml
- filename: bigid-data-posture-api-openapi.yml
  format: yaml
  label: BigID Data Posture API
  slug: bigid-data-posture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-posture-api-openapi.yml
- filename: bigid-dsar-api-openapi.yml
  format: yaml
  label: BigID DSAR API
  slug: bigid-dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-dsar-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bigid.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bigid.tools
  spf: false
hosts:
- cert_expires: Sep 30 15:26:18 2026 GMT
  host: bigid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 10:43:20 2026 GMT
  host: developer.bigid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: sandbox.bigid.tools
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bigid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BigID
provider_slug: bigid
slug: bigid-domain-security
source_filename: bigid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:26:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bigid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:43:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.bigid.tools\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bigid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bigid.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/security/bigid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Security
- DSPM
- DLP
- Privacy
- AI Security
- Data Catalog
- DSAR
- Data Discovery
- Compliance
---
