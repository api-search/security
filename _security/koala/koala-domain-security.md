---
api_specs:
- filename: koala-server-side-api-openapi.yml
  format: yaml
  label: Koala Server-Side Batch API
  slug: koala-server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala/refs/heads/main/openapi/koala-server-side-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getkoala.com
  spf: true
hosts:
- cert_expires: Sep 15 16:00:11 2026 GMT
  host: getkoala.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:43:14 2026 GMT
  host: api2.getkoala.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koala, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Koala
provider_slug: koala
slug: koala-domain-security
source_filename: koala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:00:11 2026 GMT\n  hsts: false\n- host: api2.getkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:43:14 2026 GMT\n  hsts: null\ndomains:\n- domain: getkoala.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koala/refs/heads/main/security/koala-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- B2B
- Intent Data
- Buyer Signals
- Lead Routing
- Sales Intelligence
- Visitor Identification
- Product-Led Growth
- Account Scoring
---
