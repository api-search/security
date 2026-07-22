---
api_specs:
- filename: nobueno-openapi-original.json
  format: json
  label: Jungle API
  slug: jungle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nobueno/refs/heads/main/openapi/nobueno-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nobueno.com
  spf: true
hosts:
- cert_expires: Sep 24 05:16:15 2026 GMT
  host: nobueno.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.nobueno.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nobueno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NoBueno, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NoBueno
provider_slug: nobueno
slug: nobueno-domain-security
source_filename: nobueno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nobueno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nobueno.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nobueno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nobueno/refs/heads/main/security/nobueno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jobs
- Recruiting
- Hiring
- Talent
- Matching
- Human Resources
- Candidates
---
