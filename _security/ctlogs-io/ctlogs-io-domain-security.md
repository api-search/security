---
api_specs:
- filename: ctlogs-io-certs-api-openapi.yml
  format: yaml
  label: CTlogs.io Certs API
  slug: ctlogs-io-certs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-certs-api-openapi.yml
- filename: ctlogs-io-me-api-openapi.yml
  format: yaml
  label: CTlogs.io Me API
  slug: ctlogs-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-me-api-openapi.yml
- filename: ctlogs-io-search-api-openapi.yml
  format: yaml
  label: CTlogs.io Search API
  slug: ctlogs-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-search-api-openapi.yml
- filename: ctlogs-io-stats-api-openapi.yml
  format: yaml
  label: CTlogs.io Stats API
  slug: ctlogs-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-stats-api-openapi.yml
- filename: ctlogs-io-subdomains-api-openapi.yml
  format: yaml
  label: CTlogs.io Subdomains API
  slug: ctlogs-io-subdomains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-subdomains-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ctlogs.io
  spf: true
hosts:
- cert_expires: Jan  9 10:36:07 2027 GMT
  host: ctlogs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CTlogs.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CTlogs.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CTlogs.io
provider_slug: ctlogs-io
slug: ctlogs-io-domain-security
source_filename: ctlogs-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ctlogs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 10:36:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ctlogs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ctlogs-io/security/ctlogs-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Certificate Transparency
- TLS Certificates
- SSL
- Security
- PKI
- Domains
- MCP
---
