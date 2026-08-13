---
api_specs:
- filename: covatic-audience-builder-openapi.yml
  format: yaml
  label: Covatic Audience Builder API
  slug: covatic-audience-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-audience-builder-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: covatic.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: covatic.io
  spf: false
hosts:
- cert_expires: Nov  2 12:40:39 2026 GMT
  host: covatic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: prodaudiencebuilderapi.covatic.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr  3 23:59:59 2023 GMT
  cert_issuer: ZeroSSL RSA Domain Secure Site CA
  cert_not_before: Jan  3 00:00:00 2023 GMT
  cert_subject: CN=docs.covatic.com
  host: docs.covatic.com
  hsts: null
  https: false
  https_error: certificate has expired
  note: FINDING — the documentation host Covatic publishes on covatic.com/technical/ has served an EXPIRED TLS certificate since 2023-04-03. Every modern browser and every default HTTP client refuses the connection (curl exits 60, "certificate has expired"); the host only answers with certificate verification disabled, and then 301s to https://docs.covatic.io/login. Probed 2026-08-12.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Covatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covatic, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Covatic
provider_slug: covatic
slug: covatic-domain-security
source_filename: covatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 12:40:39 2026 GMT\n  hsts: false\n- host: prodaudiencebuilderapi.covatic.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: docs.covatic.com\n  https: false\n  https_error: certificate has expired\n  tls_version: TLSv1.2\n  cert_subject: CN=docs.covatic.com\n  cert_issuer: ZeroSSL RSA Domain Secure Site CA\n  cert_not_before: Jan  3 00:00:00 2023 GMT\n  cert_expires: Apr  3 23:59:59 2023 GMT\n  hsts: null\n  note: >-\n    FINDING — the documentation host Covatic publishes on covatic.com/technical/ has\n    served an EXPIRED TLS certificate since 2023-04-03. Every modern browser and every\n    default HTTP client refuses the connection (curl exits 60, \"certificate has\n    expired\"); the host only answers with certificate verification\
  \ disabled, and then\n    301s to https://docs.covatic.io/login. Probed 2026-08-12.\ndomains:\n- domain: covatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: covatic.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/security/covatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising Technology
- AdTech
- Audience Intelligence
- Data Management Platform
- Connected TV
- Privacy
- On-Device Processing
- Attribution
- Audio
- Campaigns
- Retargeting
- Publishing
- Broadcasting
- Media
- B Corp
- United Kingdom
---
