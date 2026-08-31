---
api_specs:
- filename: superdial-api-openapi.yml
  format: yaml
  label: SuperDial API
  slug: superdial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/openapi/superdial-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: superdial.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gateway.dev
  spf: true
hosts:
- cert_expires: Oct 19 23:56:57 2026 GMT
  host: www.superdial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 07:16:39 2026 GMT
  host: docs.superdial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:15 2026 GMT
  host: robodialer-service-api-9nc4t1p9.uc.gateway.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superdial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperDial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SuperDial
provider_slug: superdial
slug: superdial-domain-security
source_filename: superdial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superdial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:56:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.superdial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 07:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: robodialer-service-api-9nc4t1p9.uc.gateway.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:15 2026 GMT\n  hsts: null\ndomains:\n- domain: superdial.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gateway.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/security/superdial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Voice AI
- Insurance
- Artificial Intelligence
- Claims
- Prior Authorization
- Benefits Verification
- Automation
---
