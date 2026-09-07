---
api_specs:
- filename: 3vjia-technology-open-platform-openapi.yml
  format: yaml
  label: 3vjia Open Platform API
  slug: 3vjia-technology-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/openapi/3vjia-technology-open-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3vjia.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.3vjia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: dev.3vjia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: open-gateway.3vjia.com
  hsts: false
  https: true
  note: 'The automated probe recorded https:false because the host is INTERMITTENTLY UNREACHABLE from a United States vantage point — roughly one attempt in three timed out at 15-25s on 2026-09-05. When it does answer it serves HTTP/2 over valid TLS (verified 2026-09-05, ssl_verify_result 0, response headers serve-vendor: ali). Corrected by hand from a repeated manual probe; this is a cross-border reachability characteristic, not a missing TLS configuration.'
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 3Vjia Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3vjia Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3vjia Technology
provider_slug: 3vjia-technology
slug: 3vjia-technology-domain-security
source_filename: 3vjia-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3vjia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n- host: dev.3vjia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n- host: open-gateway.3vjia.com\n  https: true\n  note: >-\n    The automated probe recorded https:false because the host is INTERMITTENTLY UNREACHABLE from a\n    United States vantage point — roughly one attempt in three timed out at 15-25s on 2026-09-05.\n    When it does answer it serves HTTP/2 over valid TLS (verified 2026-09-05, ssl_verify_result 0,\n    response headers serve-vendor: ali). Corrected by hand from a repeated manual probe; this is a\n    cross-border reachability characteristic, not a missing TLS configuration.\n  hsts: false\ndomains:\n- domain: 3vjia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/security/3vjia-technology-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- 3D Design
- Home Furnishing
- Interior Design
- Manufacturing
- Custom Furniture
- CAD
- Rendering
- Artificial Intelligence
- SaaS
- China
- Open Platform
---
