---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: State Department Consular Affairs API
  slug: state-dept-consular-affairs
  spec_type: OpenAPI
  url: https://cadataapi.state.gov/
- filename: openapi.yaml
  format: yaml
  label: State Department Travel Advisories
  slug: state-dept-travel-advisories
  spec_type: OpenAPI
  url: https://cadataapi.state.gov/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: state.gov
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.state.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:35:27 2026 GMT
  host: cadataapi.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: travel.state.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: State Dept Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Department, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: State Department
provider_slug: state-dept
slug: state-dept-domain-security
source_filename: state-dept-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: cadataapi.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:35:27 2026 GMT\n  hsts: null\n- host: travel.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: state.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-dept/refs/heads/main/security/state-dept-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- US Government
- Travel
- Passports
- Visas
- Travel Advisories
- Consular Affairs
- Foreign Policy
- Diplomatic
- Country Information
- Public Safety
---
