---
api_specs:
- filename: figure-heloc-inquiries-openapi-original.yml
  format: yaml
  label: HELOC Inquiries
  slug: heloc-inquiries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-heloc-inquiries-openapi-original.yml
- filename: figure-heloc-pre-qualification-openapi-original.yml
  format: yaml
  label: HELOC Pre-qualification
  slug: heloc-pre-qualification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-heloc-pre-qualification-openapi-original.yml
- filename: figure-portfolio-manager-openapi-original.yml
  format: yaml
  label: Portfolio Manager
  slug: portfolio-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-portfolio-manager-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figure.com
  spf: true
hosts:
- cert_expires: Sep 14 20:22:02 2026 GMT
  host: www.figure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:14:18 2026 GMT
  host: api.test.figure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:59:23 2026 GMT
  host: api.figure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figure
provider_slug: figure
slug: figure-domain-security
source_filename: figure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.test.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:14:18 2026 GMT\n  hsts: null\n- host: api.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:59:23 2026 GMT\n  hsts: null\ndomains:\n- domain: figure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/security/figure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- HELOC
- Home Equity
- Mortgage
- Loan Origination
- Webhooks
- Capital Markets
---
