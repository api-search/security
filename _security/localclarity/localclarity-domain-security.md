---
api_specs:
- filename: localclarity-openapi.yml
  format: yaml
  label: LocalClarity REST API
  slug: localclarity-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localclarity/refs/heads/main/openapi/localclarity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: localclarity.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tyk.io
  spf: true
hosts:
- cert_expires: Sep 15 00:13:35 2026 GMT
  host: www.localclarity.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:00:48 2026 GMT
  host: dev.localclarity.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: localclarity.cloud.tyk.io
  https: false
kind: domain-security
layout: security
method: probed
name: Localclarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalClarity, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LocalClarity
provider_slug: localclarity
slug: localclarity-domain-security
source_filename: localclarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.localclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:13:35 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: dev.localclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: localclarity.cloud.tyk.io\n  https: false\ndomains:\n- domain: localclarity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tyk.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localclarity/refs/heads/main/security/localclarity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Local SEO
- Google Business Profile
- Review Management
- Local Search
- Listings Management
- Reputation Management
- Local Marketing
- Business Listings
- Location Data
- Sentiment Analysis
- Multi-Location Brands
- Marketing
---
