---
api_specs:
- filename: done-asn-lookup-api-openapi.yml
  format: yaml
  label: _done asn lookup API
  slug: done-asn-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-asn-lookup-api-openapi.yml
- filename: done-data-api-openapi.yml
  format: yaml
  label: _done Data API
  slug: done-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-data-api-openapi.yml
- filename: done-directory-submission-api-openapi.yml
  format: yaml
  label: _done directory submission API
  slug: done-directory-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-directory-submission-api-openapi.yml
- filename: done-dmarc-api-openapi.yml
  format: yaml
  label: _done Dmarc API
  slug: done-dmarc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-dmarc-api-openapi.yml
- filename: done-ens-api-openapi.yml
  format: yaml
  label: _done Ens API
  slug: done-ens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-ens-api-openapi.yml
- filename: done-hacker-news-api-openapi.yml
  format: yaml
  label: _done hacker news API
  slug: done-hacker-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-hacker-news-api-openapi.yml
- filename: done-http-request-api-openapi.yml
  format: yaml
  label: _done http request API
  slug: done-http-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-http-request-api-openapi.yml
- filename: done-json-api-openapi.yml
  format: yaml
  label: _done JSON API
  slug: done-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-json-api-openapi.yml
- filename: done-leetspeak-api-openapi.yml
  format: yaml
  label: _done Leetspeak API
  slug: done-leetspeak-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-leetspeak-api-openapi.yml
- filename: done-mortgage-calculator-api-openapi.yml
  format: yaml
  label: _done mortgage calculator API
  slug: done-mortgage-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-mortgage-calculator-api-openapi.yml
- filename: done-ocr-api-openapi.yml
  format: yaml
  label: _done Ocr API
  slug: done-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-ocr-api-openapi.yml
- filename: done-port-scanner-api-openapi.yml
  format: yaml
  label: _done port scanner API
  slug: done-port-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-port-scanner-api-openapi.yml
- filename: done-qr-code-api-openapi.yml
  format: yaml
  label: _done qr code API
  slug: done-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-qr-code-api-openapi.yml
- filename: done-seo-api-openapi.yml
  format: yaml
  label: _done Seo API
  slug: done-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-seo-api-openapi.yml
- filename: done-sha256-hash-api-openapi.yml
  format: yaml
  label: _done sha256 hash API
  slug: done-sha256-hash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-sha256-hash-api-openapi.yml
- filename: done-shopify-rank-api-openapi.yml
  format: yaml
  label: _done shopify rank API
  slug: done-shopify-rank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-shopify-rank-api-openapi.yml
- filename: done-validation-api-openapi.yml
  format: yaml
  label: _done Validation API
  slug: done-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-validation-api-openapi.yml
- filename: done-website-screenshot-api-openapi.yml
  format: yaml
  label: _done website screenshot API
  slug: done-website-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-website-screenshot-api-openapi.yml
- filename: done-network-api-openapi.yml
  format: yaml
  label: _done Network API
  slug: done-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/openapi/done-network-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: underscoredone.com
  spf: false
hosts:
- cert_expires: Oct 20 03:00:05 2026 GMT
  host: underscoredone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 03:00:05 2026 GMT
  host: asn-lookup.underscoredone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 03:00:05 2026 GMT
  host: json-suite.underscoredone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Done Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for _done, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: _done
provider_slug: done
slug: done-domain-security
source_filename: done-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: underscoredone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:00:05 2026 GMT\n  hsts: null\n- host: asn-lookup.underscoredone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:00:05 2026 GMT\n  hsts: false\n- host: json-suite.underscoredone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:00:05 2026 GMT\n  hsts: false\ndomains:\n- domain: underscoredone.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/done/refs/heads/main/security/done-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Tools
- Utility APIs
- AI Agents
- Agent-Native
- x402
- pay-per-call
- Web3
- Crypto Payments
- DNS
- Domains
- Email Security
- Network Security
- SEO
- OCR
- Data
- fintech-calculators
---
