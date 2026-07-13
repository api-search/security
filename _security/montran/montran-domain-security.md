---
api_specs:
- filename: montran-global-payments-hub-openapi.yml
  format: yaml
  label: Montran Global Payments Hub
  slug: montran-global-payments-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-global-payments-hub-openapi.yml
- filename: montran-instant-payments-gateway-openapi.yml
  format: yaml
  label: Montran Instant Payments Gateway
  slug: montran-instant-payments-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-instant-payments-gateway-openapi.yml
- filename: montran-payments-connectivity-openapi.yml
  format: yaml
  label: Montran Payments Connectivity
  slug: montran-payments-connectivity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-payments-connectivity-openapi.yml
- filename: montran-corporate-payments-portal-openapi.yml
  format: yaml
  label: Montran Corporate Payments Portal
  slug: montran-corporate-payments-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-corporate-payments-portal-openapi.yml
- filename: montran-virtual-accounts-openapi.yml
  format: yaml
  label: Montran Virtual Accounts
  slug: montran-virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-virtual-accounts-openapi.yml
- filename: montran-sanctions-screening-openapi.yml
  format: yaml
  label: Montran Sanctions Screening
  slug: montran-sanctions-screening
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/openapi/montran-sanctions-screening-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: montran.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.montran.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.montran.com
  https: false
kind: domain-security
layout: security
method: probed
name: Montran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Montran, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Montran
provider_slug: montran
slug: montran-domain-security
source_filename: montran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.montran.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.montran.com\n  https: false\ndomains:\n- domain: montran.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/security/montran-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
---
