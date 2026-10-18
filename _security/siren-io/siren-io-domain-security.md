---
api_specs:
- filename: siren-io-collections-api-openapi.yml
  format: yaml
  label: Siren Collections API
  slug: siren-io-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-collections-api-openapi.yml
- filename: siren-io-entity-tables-api-openapi.yml
  format: yaml
  label: Siren Entity Tables API
  slug: siren-io-entity-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-entity-tables-api-openapi.yml
- filename: siren-io-generate-query-api-openapi.yml
  format: yaml
  label: Siren Generate Query API
  slug: siren-io-generate-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-generate-query-api-openapi.yml
- filename: siren-io-health-api-openapi.yml
  format: yaml
  label: Siren Health API
  slug: siren-io-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-health-api-openapi.yml
- filename: siren-io-operations-api-openapi.yml
  format: yaml
  label: Siren Operations API
  slug: siren-io-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-operations-api-openapi.yml
- filename: siren-io-status-api-openapi.yml
  format: yaml
  label: Siren Status API
  slug: siren-io-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/openapi/siren-io-status-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@siren.io"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: siren.io
  spf: true
hosts:
- cert_expires: Nov 27 03:23:16 2026 GMT
  host: siren.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Siren Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siren, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Siren
provider_slug: siren-io
slug: siren-io-domain-security
source_filename: siren-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siren.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:23:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: siren.io\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@siren.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siren-io/refs/heads/main/security/siren-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Investigative Intelligence
- Search
- Link Analysis
- Elasticsearch
- Data Analytics
---
