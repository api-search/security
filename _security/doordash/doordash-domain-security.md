---
api_specs:
- filename: doordash-drive-openapi.yml
  format: yaml
  label: DoorDash Drive API
  slug: drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-drive-openapi.yml
- filename: doordash-drive-classic-openapi.yml
  format: yaml
  label: DoorDash Drive Classic API
  slug: drive-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-drive-classic-openapi.yml
- filename: doordash-marketplace-openapi.yml
  format: yaml
  label: DoorDash Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-marketplace-openapi.yml
- filename: doordash-item-management-openapi.yml
  format: yaml
  label: DoorDash Item Management API
  slug: marketplace-item-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-item-management-openapi.yml
- filename: doordash-reporting-openapi.yml
  format: yaml
  label: DoorDash Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-reporting-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@doordash.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doordash.com
  spf: true
hosts:
- cert_expires: Sep  8 03:29:44 2026 GMT
  host: www.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:44:30 2026 GMT
  host: developer.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:44:30 2026 GMT
  host: openapi.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doordash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doordash, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: doordash
provider_slug: doordash
slug: doordash-domain-security
source_filename: doordash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:29:44 2026 GMT\n  hsts: null\n- host: developer.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:30 2026 GMT\n  hsts: null\n- host: openapi.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:30 2026 GMT\n  hsts: null\ndomains:\n- domain: doordash.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@doordash.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/security/doordash-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags: []
---
