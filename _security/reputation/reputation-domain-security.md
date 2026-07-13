---
api_specs:
- filename: reputation-api-openapi.yml
  format: yaml
  label: Reputation API
  slug: reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reputation.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: reputation-api.com
  spf: false
hosts:
- cert_expires: Sep 15 20:47:22 2026 GMT
  host: reputation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 09:29:22 2026 GMT
  host: apidocs.reputation.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: reputation-api.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reputation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reputation, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reputation
provider_slug: reputation
slug: reputation-domain-security
source_filename: reputation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reputation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.reputation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:29:22 2026 GMT\n  hsts: null\n- host: reputation-api.com\n  https: false\ndomains:\n- domain: reputation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: reputation-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/security/reputation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
---
