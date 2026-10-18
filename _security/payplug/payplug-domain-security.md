---
api_specs:
- filename: payplug-cards-api-openapi.yml
  format: yaml
  label: PayPlug Cards API
  slug: payplug-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payplug/refs/heads/main/openapi/payplug-cards-api-openapi.yml
- filename: payplug-installment-plans-api-openapi.yml
  format: yaml
  label: PayPlug Installment Plans API
  slug: payplug-installment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payplug/refs/heads/main/openapi/payplug-installment-plans-api-openapi.yml
- filename: payplug-payments-api-openapi.yml
  format: yaml
  label: PayPlug Payments API
  slug: payplug-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payplug/refs/heads/main/openapi/payplug-payments-api-openapi.yml
- filename: payplug-payplug-api-api-openapi.yml
  format: yaml
  label: PayPlug PayPlug API
  slug: payplug-payplug-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payplug/refs/heads/main/openapi/payplug-payplug-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: payplug.com
  spf: true
hosts:
- cert_expires: Dec 31 15:23:42 2026 GMT
  host: www.payplug.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Payplug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayPlug, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PayPlug
provider_slug: payplug
slug: payplug-domain-security
source_filename: payplug-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payplug.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 15:23:42 2026 GMT\n  hsts: null\ndomains:\n- domain: payplug.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payplug/refs/heads/main/security/payplug-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
