---
api_specs:
- filename: synthient-account-api-openapi.yml
  format: yaml
  label: Synthient API Account API
  slug: synthient-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-account-api-openapi.yml
- filename: synthient-anonymizers-api-openapi.yml
  format: yaml
  label: Synthient API Anonymizers API
  slug: synthient-anonymizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-anonymizers-api-openapi.yml
- filename: synthient-helios-api-openapi.yml
  format: yaml
  label: Synthient API Helios API
  slug: synthient-helios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-helios-api-openapi.yml
- filename: synthient-ja4t-api-openapi.yml
  format: yaml
  label: Synthient API JA4T API
  slug: synthient-ja4t-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-ja4t-api-openapi.yml
- filename: synthient-lookup-api-openapi.yml
  format: yaml
  label: Synthient API Lookup API
  slug: synthient-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-lookup-api-openapi.yml
- filename: synthient-proxies-api-openapi.yml
  format: yaml
  label: Synthient API Proxies API
  slug: synthient-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-proxies-api-openapi.yml
- filename: synthient-torrents-api-openapi.yml
  format: yaml
  label: Synthient API Torrents API
  slug: synthient-torrents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-torrents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synthient.com
  spf: true
hosts:
- cert_expires: Dec 23 03:47:02 2026 GMT
  host: synthient.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synthient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthient API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Synthient API
provider_slug: synthient
slug: synthient-domain-security
source_filename: synthient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synthient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 03:47:02 2026 GMT\n  hsts: null\ndomains:\n- domain: synthient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/security/synthient-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IP
- Enrichment
- Cybersecurity
- Data
---
