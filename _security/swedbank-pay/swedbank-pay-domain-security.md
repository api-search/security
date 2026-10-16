---
api_specs:
- filename: swedbank-pay-openapi-generated.yml
  format: yaml
  label: Swedbank Pay API
  slug: swedbank-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swedbank-pay/refs/heads/main/openapi/_ae-authored/swedbank-pay-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swedbankpay.com
  spf: true
hosts:
- cert_expires: Dec 15 12:16:02 2026 GMT
  host: swedbankpay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swedbank Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swedbank Pay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swedbank Pay
provider_slug: swedbank-pay
slug: swedbank-pay-domain-security
source_filename: swedbank-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swedbankpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 12:16:02 2026 GMT\n  hsts: false\ndomains:\n- domain: swedbankpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swedbank-pay/refs/heads/main/security/swedbank-pay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- FinTech
- API
- Nordic
---
