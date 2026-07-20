---
api_specs:
- filename: cabify-ride-hailing-openapi.yml
  format: yaml
  label: Cabify Ride-Hailing API
  slug: cabify-ride-hailing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-ride-hailing-openapi.yml
- filename: cabify-logistics-openapi.yml
  format: yaml
  label: Cabify Logistics API
  slug: cabify-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-logistics-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "letsencrypt.org"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cabify.com
  spf: true
hosts:
- cert_expires: Sep 29 15:28:06 2026 GMT
  host: cabify.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 02:40:20 2026 GMT
  host: developers.cabify.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 15:28:06 2026 GMT
  host: logistics.api.cabify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cabify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cabify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cabify
provider_slug: cabify
slug: cabify-domain-security
source_filename: cabify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:28:06 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: developers.cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: logistics.api.cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:28:06 2026 GMT\n  hsts: null\ndomains:\n- domain: cabify.com\n  dnssec: true\n  caa:\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/security/cabify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Ride Hailing
- Mobility
- Logistics
- Delivery
- Last Mile Delivery
- Webhooks
- OAuth
---
