---
api_specs:
- filename: ripe-insurance-umbraco-content-delivery-openapi.json
  format: json
  label: Ripe Insurance Umbraco Content Delivery API
  slug: ripe-insurance-umbraco-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-umbraco-content-delivery-openapi.json
- filename: ripe-insurance-cycleplan-content-delivery-openapi.json
  format: json
  label: Cycleplan Umbraco Content Delivery API
  slug: ripe-insurance-cycleplan-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ripeinsurance.co.uk
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.ripeinsurance.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ripe Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ripe Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ripe Insurance
provider_slug: ripe-insurance
slug: ripe-insurance-domain-security
source_filename: ripe-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ripeinsurance.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ripeinsurance.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/security/ripe-insurance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Managing General Agent
- Specialist Insurance
- Personal Lines
- Small Business Insurance
- Underwriting
- Direct to Consumer
- Broker
---
