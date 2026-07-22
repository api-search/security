---
api_specs:
- filename: simplifi-simplifipay-openapi.yml
  format: yaml
  label: SimpliFi Cards API
  slug: simplifi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplifipay.com
  spf: true
hosts:
- cert_expires: Sep 15 09:42:45 2026 GMT
  host: simplifipay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplifi Simplifipay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplifi/Simplifipay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simplifi/Simplifipay
provider_slug: simplifi-simplifipay
slug: simplifi-simplifipay-domain-security
source_filename: simplifi-simplifipay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplifipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:42:45 2026 GMT\n  hsts: false\ndomains:\n- domain: simplifipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/security/simplifi-simplifipay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cards
- Card Issuing
- Virtual Cards
- Fintech
- Payments
- Banking as a Service
- Embedded Finance
- GCC
- Webhooks
---
