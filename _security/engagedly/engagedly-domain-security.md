---
api_specs:
- filename: engagedly-openapi.yml
  format: yaml
  label: Engagedly API
  slug: engagedly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: engagedly.com
  spf: true
hosts:
- cert_expires: Aug 24 05:58:02 2026 GMT
  host: engagedly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: api.engagedly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Engagedly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engagedly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Engagedly
provider_slug: engagedly
slug: engagedly-domain-security
source_filename: engagedly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engagedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:58:02 2026 GMT\n  hsts: false\n- host: api.engagedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: engagedly.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/security/engagedly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Performance Management
- HR Software
- Employee Engagement
- Goal Tracking
- 360 Feedback
- Learning Management
- Employee Recognition
- Talent Management
- OKR
- People Operations
---
