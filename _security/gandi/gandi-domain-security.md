---
api_specs:
- filename: gandi-authorization-api-openapi.yml
  format: yaml
  label: Gandi Authorization API
  slug: gandi-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-authorization-api-openapi.yml
- filename: gandi-availability-api-openapi.yml
  format: yaml
  label: Gandi Availability API
  slug: gandi-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-availability-api-openapi.yml
- filename: gandi-dnssec-api-openapi.yml
  format: yaml
  label: Gandi DNSSEC API
  slug: gandi-dnssec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-dnssec-api-openapi.yml
- filename: gandi-domains-api-openapi.yml
  format: yaml
  label: Gandi Domains API
  slug: gandi-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-domains-api-openapi.yml
- filename: gandi-ownership-api-openapi.yml
  format: yaml
  label: Gandi Ownership API
  slug: gandi-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-ownership-api-openapi.yml
- filename: gandi-records-api-openapi.yml
  format: yaml
  label: Gandi Records API
  slug: gandi-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-records-api-openapi.yml
- filename: gandi-renewal-api-openapi.yml
  format: yaml
  label: Gandi Renewal API
  slug: gandi-renewal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-renewal-api-openapi.yml
- filename: gandi-trademark-api-openapi.yml
  format: yaml
  label: Gandi Trademark API
  slug: gandi-trademark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-trademark-api-openapi.yml
- filename: gandi-tsig-api-openapi.yml
  format: yaml
  label: Gandi TSIG API
  slug: gandi-tsig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-tsig-api-openapi.yml
- filename: gandi-utilities-api-openapi.yml
  format: yaml
  label: Gandi Utilities API
  slug: gandi-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-utilities-api-openapi.yml
- filename: gandi-zone-transfers-api-openapi.yml
  format: yaml
  label: Gandi Zone Transfers API
  slug: gandi-zone-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-zone-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gandi.net
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.gandi.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.gandi.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.sandbox.gandi.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gandi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gandi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gandi
provider_slug: gandi
slug: gandi-domain-security
source_filename: gandi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.sandbox.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: gandi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/security/gandi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- DNS
- Domains
- Domain Registrar
- Email
- Hosting
- Certificates
---
