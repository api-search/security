---
api_specs:
- filename: api-reference
  format: yaml
  label: OpenMetadata REST API
  slug: openmetadata-rest-api
  spec_type: OpenAPI
  url: https://docs.open-metadata.org/api-reference
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: open-metadata.org
  spf: true
hosts:
- cert_expires: Aug 29 18:13:50 2026 GMT
  host: open-metadata.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:20:30 2026 GMT
  host: docs.open-metadata.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openmetadata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenMetadata, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenMetadata
provider_slug: openmetadata
slug: openmetadata-domain-security
source_filename: openmetadata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-metadata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.open-metadata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: open-metadata.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmetadata/refs/heads/main/security/openmetadata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Catalog
- Metadata
- Data Governance
- Data Lineage
- Data Quality
- Open Source
- Data Discovery
- Data Observability
---
