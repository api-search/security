---
api_specs:
- filename: collate-openmetadata-openapi.yml
  format: yaml
  label: OpenMetadata REST API
  slug: collate-openmetadata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collate/refs/heads/main/openapi/collate-openmetadata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: collate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: open-metadata.org
  spf: true
hosts:
- cert_expires: Sep  7 05:28:59 2026 GMT
  host: collate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:20:30 2026 GMT
  host: docs.open-metadata.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: sandbox.open-metadata.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Collate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Collate
provider_slug: collate
slug: collate-domain-security
source_filename: collate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:28:59 2026 GMT\n  hsts: false\n- host: docs.open-metadata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.open-metadata.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: collate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: open-metadata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collate/refs/heads/main/security/collate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Metadata
- Data Catalog
- Data Governance
- Data Discovery
- Data Quality
- Data Lineage
- Open Source
- API
---
