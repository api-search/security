---
api_specs:
- filename: beazley-data-capture-quote-and-risk-data-v2.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v2'
  slug: beazley-data-capture-quote-and-risk-data-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data-v2.yml
- filename: beazley-data-capture-quote-and-risk-data.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v1'
  slug: beazley-data-capture-quote-and-risk-data-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data.yml
- filename: beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
  format: yaml
  label: 'Beazley Data Capture: Quote and Risk Data v3 (pre-release)'
  slug: beazley-data-capture-quote-and-risk-data-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-data-capture-quote-and-risk-data-v3-pre-release.yml
- filename: beazley-compliance-web-api.yml
  format: yaml
  label: Beazley Compliance Web API
  slug: beazley-compliance-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-compliance-web-api.yml
- filename: beazley-broker-and-insured-marketing-data-v2.yml
  format: yaml
  label: Beazley Broker and Insured Marketing Data v2
  slug: beazley-broker-and-insured-marketing-data-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-broker-and-insured-marketing-data-v2.yml
- filename: beazley-currency-exchange.yml
  format: yaml
  label: Beazley Currency Exchange
  slug: beazley-currency-exchange
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-currency-exchange.yml
- filename: beazley-about-beazley.yml
  format: yaml
  label: About Beazley
  slug: beazley-about-beazley
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-about-beazley.yml
- filename: beazley-fast-reader.yml
  format: yaml
  label: Beazley Fast Reader
  slug: beazley-fast-reader
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-fast-reader.yml
- filename: beazley-simple-raters.yml
  format: yaml
  label: Beazley Simple Raters
  slug: beazley-simple-raters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-simple-raters.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beazley.com
  spf: true
hosts:
- cert_expires: Oct  7 14:39:29 2026 GMT
  host: www.beazley.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: developer.beazley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.beazley.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beazley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beazley, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beazley
provider_slug: beazley
slug: beazley-domain-security
source_filename: beazley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beazley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:39:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.beazley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.beazley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: beazley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/security/beazley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Cyber Insurance
- Specialty Insurance
- Lloyd's of London
- Underwriting
- Risk Data
- Broker
- Carrier
---
