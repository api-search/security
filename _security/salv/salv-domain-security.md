---
api_specs:
- filename: salv-aml-openapi-original.yml
  format: yaml
  label: Salv AML API
  slug: salv-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-aml-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: salv.com
  spf: true
hosts:
- cert_expires: Oct 15 17:00:16 2026 GMT
  host: salv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Salv
provider_slug: salv
slug: salv-domain-security
source_filename: salv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:00:16 2026 GMT\n  hsts: false\ndomains:\n- domain: salv.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/security/salv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Anti-Money Laundering
- Financial Crime
- Compliance
- RegTech
- Sanctions Screening
- Transaction Monitoring
- Fraud Prevention
---
