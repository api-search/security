---
api_specs:
- filename: healthsherpa-enrollment-sessions-api-openapi.yml
  format: yaml
  label: HealthSherpa Enrollment Sessions API
  slug: healthsherpa-enrollment-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-enrollment-sessions-api-openapi.yml
- filename: healthsherpa-enrollments-api-openapi.yml
  format: yaml
  label: HealthSherpa Enrollments API
  slug: healthsherpa-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-enrollments-api-openapi.yml
- filename: healthsherpa-quotes-api-openapi.yml
  format: yaml
  label: HealthSherpa Quotes API
  slug: healthsherpa-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-quotes-api-openapi.yml
- filename: healthsherpa-reference-api-openapi.yml
  format: yaml
  label: HealthSherpa Reference API
  slug: healthsherpa-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-reference-api-openapi.yml
- filename: healthsherpa-utility-api-openapi.yml
  format: yaml
  label: HealthSherpa Utility API
  slug: healthsherpa-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: healthsherpa.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.one.healthsherpa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthsherpa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthSherpa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HealthSherpa
provider_slug: healthsherpa
slug: healthsherpa-domain-security
source_filename: healthsherpa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.one.healthsherpa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: healthsherpa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/security/healthsherpa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health Insurance
- Healthcare
- ACA
- Enrollment
- Quoting
- Insurance
- Enhanced Direct Enrollment
- ICHRA
---
