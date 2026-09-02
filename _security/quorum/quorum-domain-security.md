---
api_specs:
- filename: quorum-divisionorders-api-openapi.yml
  format: yaml
  label: Quorum Software DivisionOrders API
  slug: quorum-divisionorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-divisionorders-api-openapi.yml
- filename: quorum-leases-api-openapi.yml
  format: yaml
  label: Quorum Software Leases API
  slug: quorum-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-leases-api-openapi.yml
- filename: quorum-owners-api-openapi.yml
  format: yaml
  label: Quorum Software Owners API
  slug: quorum-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-owners-api-openapi.yml
- filename: quorum-tracts-api-openapi.yml
  format: yaml
  label: Quorum Software Tracts API
  slug: quorum-tracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-tracts-api-openapi.yml
- filename: quorum-wells-api-openapi.yml
  format: yaml
  label: Quorum Software Wells API
  slug: quorum-wells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-wells-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quorumsoftware.com
  spf: true
hosts:
- cert_expires: Sep 29 03:42:15 2026 GMT
  host: www.quorumsoftware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.quorumsoftware.com
  https: false
kind: domain-security
layout: security
method: probed
name: Quorum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quorum Software, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quorum Software
provider_slug: quorum
slug: quorum-domain-security
source_filename: quorum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quorumsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.quorumsoftware.com\n  https: false\ndomains:\n- domain: quorumsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/security/quorum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil and Gas
- Upstream
- Land Management
- Royalty Accounting
- Production Reporting
---
