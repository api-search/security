---
api_specs:
- filename: crowddev-cdp-public-openapi.yml
  format: yaml
  label: CDP Public API
  slug: cdp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-cdp-public-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowd.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lfx.dev
  spf: true
hosts:
- cert_expires: Sep 16 10:35:36 2026 GMT
  host: crowd.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 16:38:46 2026 GMT
  host: docs.crowd.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 14:57:49 2026 GMT
  host: cm.lfx.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crowddev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowd.dev, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Crowd.dev
provider_slug: crowddev
slug: crowddev-domain-security
source_filename: crowddev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowd.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:35:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.crowd.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:38:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cm.lfx.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crowd.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: lfx.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/security/crowddev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open Source
- Community Data Platform
- Open Source Intelligence
---
