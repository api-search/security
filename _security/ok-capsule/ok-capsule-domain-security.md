---
api_specs:
- filename: ok-capsule-core-api-v2-openapi.yaml
  format: yaml
  label: OK Capsule Core API V2
  slug: ok-capsule-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/openapi/ok-capsule-core-api-v2-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: okcapsule.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: okcapsule.app
  spf: false
hosts:
- cert_expires: Nov 24 08:50:17 2026 GMT
  host: okcapsule.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: docs.okcapsule.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: na1-prod.okcapsule.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ok Capsule Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OK Capsule, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OK Capsule
provider_slug: ok-capsule
slug: ok-capsule-domain-security
source_filename: ok-capsule-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okcapsule.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.okcapsule.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: na1-prod.okcapsule.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: okcapsule.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: okcapsule.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/security/ok-capsule-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Supplements
- Nutrition
- Health
- Manufacturing
- Fulfillment
- Ecommerce
- Personalization
- Orders
- Shipping
- Agents
- MCP
- Telehealth
---
