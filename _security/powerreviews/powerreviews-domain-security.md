---
api_specs:
- filename: powerreviews-readservices-openapi.yml
  format: yaml
  label: PowerReviews Read API
  slug: powerreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-readservices-openapi.yml
- filename: powerreviews-writeservices-openapi.yml
  format: yaml
  label: PowerReviews Write API
  slug: powerreviews-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-writeservices-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: powerreviews.com
  spf: true
hosts:
- cert_expires: Sep 26 11:36:35 2026 GMT
  host: www.powerreviews.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: developers.powerreviews.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: readservices-b2c.powerreviews.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powerreviews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerReviews, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PowerReviews
provider_slug: powerreviews
slug: powerreviews-domain-security
source_filename: powerreviews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.powerreviews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:36:35 2026 GMT\n  hsts: false\n- host: developers.powerreviews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: readservices-b2c.powerreviews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: powerreviews.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/security/powerreviews-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Ratings and Reviews
- User Generated Content
- Retail
- Marketing
- Syndication
- Questions and Answers
- Product Data
---
