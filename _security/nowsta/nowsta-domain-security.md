---
api_specs:
- filename: nowsta-integration-openapi.yml
  format: yaml
  label: Nowsta Integration API
  slug: nowsta-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowsta/refs/heads/main/openapi/nowsta-integration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nowsta.com
  spf: true
hosts:
- cert_expires: Sep  6 14:36:26 2026 GMT
  host: www.nowsta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:54:15 2026 GMT
  host: api.nowsta.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_observed_on: POST /integrations/v1/events/publications
  https: true
  tls_version: TLSv1.3
- host: app.nowsta.com
  https: true
  reachable: true
- host: my.nowsta.com
  https: true
  reachable: true
- host: status.nowsta.com
  https: true
  provider: Atlassian Statuspage
  reachable: true
kind: domain-security
layout: security
method: probed
name: Nowsta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nowsta, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nowsta
provider_slug: nowsta
slug: nowsta-domain-security
source_filename: nowsta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes: >-\n  The web.archive.org / archive.org rows produced by the mechanical probe were removed - they are an\n  artefact of the API humanURL pointing at the archived Nowsta developer reference (Nowsta's own docs\n  host, developer.nowsta.com, no longer resolves) and say nothing about Nowsta's security posture.\n  api.nowsta.com returns no HSTS header on the root path (which 404s), but does send\n  `Strict-Transport-Security: max-age=31536000; includeSubDomains` on the real integration paths -\n  observed 2026-08-01 on POST /integrations/v1/events/publications.\nhosts:\n- host: www.nowsta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:36:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nowsta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains:\
  \ true\n  hsts_observed_on: POST /integrations/v1/events/publications\n- host: app.nowsta.com\n  https: true\n  reachable: true\n- host: my.nowsta.com\n  https: true\n  reachable: true\n- host: status.nowsta.com\n  https: true\n  reachable: true\n  provider: Atlassian Statuspage\ndomains:\n- domain: nowsta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- id: no-dnssec\n  severity: low\n  detail: nowsta.com is not DNSSEC signed.\n- id: no-caa\n  severity: low\n  detail: >-\n    No CAA records published for nowsta.com, so certificate issuance is not constrained to named CAs.\n- id: dmarc-policy-none\n  severity: medium\n  detail: >-\n    DMARC is published but the policy is p=none (monitor only), so spoofed mail claiming to be from\n    nowsta.com is reported but not rejected or quarantined.\n- id: no-security-txt\n  severity: medium\n  detail: >-\n    No /.well-known/security.txt on any Nowsta host. www.nowsta.com answers 200 for every\n  \
  \  /.well-known/* path with the WordPress homepage (soft 404), which is a false positive, not a\n    published document - see well-known/nowsta-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowsta/refs/heads/main/security/nowsta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- workforce-management
- staff-scheduling
- shift-scheduling
- time-and-attendance
- hourly-workforce
- gig-work
- event-staffing
- hospitality
- staffing-agency
- vendor-management
- payroll
- human-resources
---
