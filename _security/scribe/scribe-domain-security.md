---
api_specs:
- filename: scribe-search-retrieval-openapi.yml
  format: yaml
  label: Scribe Search & Retrieval API
  slug: scribe-search-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scribe/refs/heads/main/openapi/scribe-search-retrieval-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scribe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scribehow.com
  spf: true
hosts:
- cert_expires: Sep 18 01:29:53 2026 GMT
  host: scribe.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:31:14 2026 GMT
  host: public-api.scribehow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scribe, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scribe
provider_slug: scribe
slug: scribe-domain-security
source_filename: scribe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: public-api.scribehow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:31:14 2026 GMT\n  hsts: null\ndomains:\n- domain: scribe.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: scribehow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scribe/refs/heads/main/security/scribe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- Documentation
- Knowledge Management
- Search
- Workflow
- Process Documentation
- Enterprise
---
