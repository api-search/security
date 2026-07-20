---
api_specs:
- filename: harver-openapi-original.json
  format: json
  label: Harver Public API
  slug: harver-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: harver.com
  spf: true
hosts:
- cert_expires: Sep 29 07:45:29 2026 GMT
  host: harver.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.harver.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Harver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harver, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Harver
provider_slug: harver
slug: harver-domain-security
source_filename: harver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:45:29 2026 GMT\n  hsts: false\n- host: api.harver.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: harver.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/security/harver-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- HR
- HR Tech
- Recruiting
- Hiring
- Talent Intelligence
- Pre-Employment Assessment
- Candidate Experience
- Applicant Tracking
---
