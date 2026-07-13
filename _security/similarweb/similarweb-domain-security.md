---
api_specs:
- filename: llms.txt
  format: yaml
  label: SimilarWeb REST API
  slug: similarweb-rest-api
  spec_type: OpenAPI
  url: https://developers.similarweb.com/llms.txt
- filename: similarweb-batch-api-openapi.yml
  format: yaml
  label: SimilarWeb Batch API
  slug: similarweb-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-batch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: similarweb.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.similarweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:15:51 2026 GMT
  host: developers.similarweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.similarweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Similarweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimilarWeb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SimilarWeb
provider_slug: similarweb
slug: similarweb-domain-security
source_filename: similarweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: developers.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: similarweb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/security/similarweb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-commerce
- SEO
---
