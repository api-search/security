---
api_specs:
- filename: healthsherpa-one-openapi.json
  format: json
  label: HealthSherpa Public API (ONE)
  slug: healthsherpa-public-api-one
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-one-openapi.json
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
