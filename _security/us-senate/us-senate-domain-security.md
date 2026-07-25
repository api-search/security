---
api_specs:
- filename: us-senate-clients-api-openapi.yml
  format: yaml
  label: US Senate Clients API
  slug: us-senate-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-clients-api-openapi.yml
- filename: us-senate-constants-api-openapi.yml
  format: yaml
  label: US Senate Constants API
  slug: us-senate-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-constants-api-openapi.yml
- filename: us-senate-contributions-api-openapi.yml
  format: yaml
  label: US Senate Contributions API
  slug: us-senate-contributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-contributions-api-openapi.yml
- filename: us-senate-filings-api-openapi.yml
  format: yaml
  label: US Senate Filings API
  slug: us-senate-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-filings-api-openapi.yml
- filename: us-senate-lobbyists-api-openapi.yml
  format: yaml
  label: US Senate Lobbyists API
  slug: us-senate-lobbyists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-lobbyists-api-openapi.yml
- filename: us-senate-registrants-api-openapi.yml
  format: yaml
  label: US Senate Registrants API
  slug: us-senate-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-registrants-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: senate.gov
  spf: false
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: lda.senate.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Senate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Senate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: US Senate
provider_slug: us-senate
slug: us-senate-domain-security
source_filename: us-senate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lda.senate.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: senate.gov\n  dnssec: true\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/security/us-senate-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Lobbying
- Government Transparency
- Campaign Finance
- Open Data
---
