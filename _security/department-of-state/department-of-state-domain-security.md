---
api_specs:
- filename: department-of-state-state-gov-content-openapi.yml
  format: yaml
  label: state.gov Content API
  slug: state-gov-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-state/refs/heads/main/openapi/department-of-state-state-gov-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: state.gov
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 13:47:13 2026 GMT
  host: travel.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 10:33:24 2026 GMT
  host: step.state.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Department Of State Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of State, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of State
provider_slug: department-of-state
slug: department-of-state-domain-security
source_filename: department-of-state-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: null\n- host: travel.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:47:13 2026 GMT\n  hsts: null\n- host: step.state.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:33:24 2026 GMT\n  hsts: null\ndomains:\n- domain: state.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-state/refs/heads/main/security/department-of-state-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal-Government
- Foreign Affairs
- Travel
- Consular
- Visas
- Passports
---
