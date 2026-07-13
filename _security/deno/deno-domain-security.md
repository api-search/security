---
api_specs:
- filename: deno-deploy-rest-api-openapi.yml
  format: yaml
  label: Deno Deploy REST API
  slug: deploy-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-deploy-rest-api-openapi.yml
- filename: deno-deploy-v2-api-openapi.yml
  format: yaml
  label: Deno Deploy API V2
  slug: deploy-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-deploy-v2-api-openapi.yml
- filename: deno-subhosting-api-openapi.yml
  format: yaml
  label: Deno Subhosting API
  slug: subhosting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/openapi/deno-subhosting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deno.com
  spf: true
hosts:
- cert_expires: Aug 24 02:16:36 2026 GMT
  host: deno.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:49:21 2026 GMT
  host: dash.deno.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 11:58:39 2026 GMT
  host: docs.deno.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deno, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deno
provider_slug: deno
slug: deno-domain-security
source_filename: deno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:16:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dash.deno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:49:21 2026 GMT\n  hsts: false\n- host: docs.deno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:58:39 2026 GMT\n  hsts: false\ndomains:\n- domain: deno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/security/deno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Deployment
- Edge
- JavaScript
- Runtime
- Serverless
- TypeScript
---
