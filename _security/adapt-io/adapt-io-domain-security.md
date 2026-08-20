---
api_specs:
- filename: adapt-io-company-search-api-openapi.yml
  format: yaml
  label: Adapt Company Search API
  slug: adapt-io-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-company-search-api-openapi.yml
- filename: adapt-io-contact-enrichment-api-openapi.yml
  format: yaml
  label: Adapt Contact Enrichment API
  slug: adapt-io-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-enrichment-api-openapi.yml
- filename: adapt-io-contact-purchase-api-openapi.yml
  format: yaml
  label: Adapt Contact Purchase API
  slug: adapt-io-contact-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-purchase-api-openapi.yml
- filename: adapt-io-contact-search-api-openapi.yml
  format: yaml
  label: Adapt Contact Search API
  slug: adapt-io-contact-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adapt.io
  spf: true
hosts:
- cert_expires: Sep 19 13:02:08 2026 GMT
  host: www.adapt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 13:02:08 2026 GMT
  host: api.adapt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adapt Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adapt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adapt
provider_slug: adapt-io
slug: adapt-io-domain-security
source_filename: adapt-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adapt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:02:08 2026 GMT\n  hsts: false\n- host: api.adapt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:02:08 2026 GMT\n  hsts: null\ndomains:\n- domain: adapt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/security/adapt-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B Data
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
- Sales Acceleration
- Data Enrichment
- Prospecting
- Lead Generation
- Email Finder
- Account Based Marketing
- CRM Enrichment
- Marketing
- Sales
---
