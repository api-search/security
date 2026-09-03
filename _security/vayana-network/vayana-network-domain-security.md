---
api_specs:
- filename: vayana-network-atlas-openapi.json
  format: json
  label: Vayana Atlas API
  slug: vayana-network-atlas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vayana-network/refs/heads/main/openapi/vayana-network-atlas-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vayana.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.vayana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: atlas.vayana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: s.api.one.vayana.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vayana Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vayana Network, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vayana Network
provider_slug: vayana-network
slug: vayana-network-domain-security
source_filename: vayana-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vayana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: atlas.vayana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: s.api.one.vayana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vayana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayana-network/refs/heads/main/security/vayana-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trade Finance
- Supply Chain Finance
- Tax Compliance
- E-Invoicing
- GST
- Identity Verification
- KYC
- India
- Embedded Finance
- Government
- Logistics
---
