---
api_specs:
- filename: open-fec-candidate-api-openapi.yml
  format: yaml
  label: OpenFEC Candidate API
  slug: open-fec-candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-candidate-api-openapi.yml
- filename: open-fec-candidates-api-openapi.yml
  format: yaml
  label: OpenFEC Candidates API
  slug: open-fec-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-candidates-api-openapi.yml
- filename: open-fec-committee-api-openapi.yml
  format: yaml
  label: OpenFEC Committee API
  slug: open-fec-committee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-committee-api-openapi.yml
- filename: open-fec-committees-api-openapi.yml
  format: yaml
  label: OpenFEC Committees API
  slug: open-fec-committees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-committees-api-openapi.yml
- filename: open-fec-elections-api-openapi.yml
  format: yaml
  label: OpenFEC Elections API
  slug: open-fec-elections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-elections-api-openapi.yml
- filename: open-fec-filings-api-openapi.yml
  format: yaml
  label: OpenFEC Filings API
  slug: open-fec-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-filings-api-openapi.yml
- filename: open-fec-names-api-openapi.yml
  format: yaml
  label: OpenFEC Names API
  slug: open-fec-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-names-api-openapi.yml
- filename: open-fec-schedules-api-openapi.yml
  format: yaml
  label: OpenFEC Schedules API
  slug: open-fec-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/openapi/open-fec-schedules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fec.gov
  spf: true
hosts:
- cert_expires: Sep  6 14:21:08 2026 GMT
  host: www.fec.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 14:21:16 2026 GMT
  host: api.open.fec.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Fec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFEC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OpenFEC
provider_slug: open-fec
slug: open-fec-domain-security
source_filename: open-fec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:21:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.open.fec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:21:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fec.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-fec/refs/heads/main/security/open-fec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Campaign Finance
- Elections
- FEC
- Federal
- Government
---
