---
api_specs:
- filename: onerail-delivery-api-openapi.yml
  format: yaml
  label: OneRail Delivery API
  slug: onerail-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-delivery-api-openapi.yml
- filename: onerail-operations-api-openapi.yml
  format: yaml
  label: OneRail Operations API
  slug: onerail-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-operations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onerail.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onerail.io
  spf: true
hosts:
- cert_expires: Sep  7 16:34:23 2026 GMT
  host: www.onerail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 14:15:25 2026 GMT
  host: developer.onerail.io
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 15:04:15 2026 GMT
  host: onerail-delivery-api-prod.azurewebsites.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onerail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneRail, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OneRail
provider_slug: onerail
slug: onerail-domain-security
source_filename: onerail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onerail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:34:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.onerail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 14:15:25 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: onerail-delivery-api-prod.azurewebsites.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 15:04:15 2026 GMT\n  hsts: false\ndomains:\n- domain: onerail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: onerail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/security/onerail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- last-mile-delivery
- delivery-orchestration
- logistics
- supply-chain
- route-optimization
- courier-network
- shipping
- fleet-management
- transportation
- order-management
- webhooks
- final-mile
---
