---
api_specs:
- filename: plasmic-openapi.yml
  format: yaml
  label: Plasmic CMS API
  slug: cms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plasmic/refs/heads/main/openapi/plasmic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plasmic.app
  spf: true
hosts:
- cert_expires: Oct  8 04:03:50 2026 GMT
  host: www.plasmic.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 08:37:01 2026 GMT
  host: studio.plasmic.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:48:00 2026 GMT
  host: docs.plasmic.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plasmic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plasmic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plasmic
provider_slug: plasmic
slug: plasmic-domain-security
source_filename: plasmic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plasmic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: studio.plasmic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:37:01 2026 GMT\n  hsts: false\n- host: docs.plasmic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: plasmic.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plasmic/refs/heads/main/security/plasmic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Visual Builder
- Headless CMS
- React
- Next.js
- Gatsby
- Low-Code
- Frontend
---
