---
api_specs:
- filename: makeswift-openapi.json
  format: json
  label: Makeswift REST API
  slug: makeswift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeswift/refs/heads/main/openapi/makeswift-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: makeswift.com
  spf: true
hosts:
- cert_expires: Aug 25 14:42:00 2026 GMT
  host: makeswift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:45:14 2026 GMT
  host: api.makeswift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makeswift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Makeswift, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Makeswift
provider_slug: makeswift
slug: makeswift-domain-security
source_filename: makeswift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makeswift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:42:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.makeswift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:45:14 2026 GMT\n  hsts: null\ndomains:\n- domain: makeswift.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeswift/refs/heads/main/security/makeswift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Visual Page Builder
- Website Builder
- Next.js
- Headless CMS
- Composable
- Content Management
- Web Development
- Developer Tools
---
