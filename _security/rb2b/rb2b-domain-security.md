---
api_specs:
- filename: postman.yaml
  format: yaml
  label: RB2B Identification API
  slug: rb2b-identification-api
  spec_type: Postman
  url: https://postman.api.rb2b.com/
- filename: postman.yaml
  format: yaml
  label: RB2B Enrichment API
  slug: rb2b-enrichment-api
  spec_type: Postman
  url: https://postman.api.rb2b.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rb2b.com
  spf: true
hosts:
- cert_expires: Sep 28 07:30:47 2026 GMT
  host: www.rb2b.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:47:09 2026 GMT
  host: support.rb2b.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rb2B Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RB2B, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RB2B
provider_slug: rb2b
slug: rb2b-domain-security
source_filename: rb2b-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rb2b.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:30:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.rb2b.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: rb2b.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rb2b/refs/heads/main/security/rb2b-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Resolution
- Visitor Identification
- B2B Data
- Lead Generation
- Sales Intelligence
- Marketing
- Data Enrichment
- LinkedIn Enrichment
- Hashed Email
- Mobile Ad ID
- Firmographics
- Webhooks
- Pixel
- Adtech
- Identity Graph
---
