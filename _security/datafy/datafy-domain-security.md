---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datafy.com
  spf: true
hosts:
- cert_expires: Oct  6 10:18:29 2026 GMT
  host: www.datafy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:18:29 2026 GMT
  host: api.datafy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: 'Corrected by hand on 2026-08-12 from a direct probe. The automated pass recorded hsts: null because every request to this host returns HTTP 500 (UnauthorizedError) and the header was not read off a non-2xx response; `curl -I https://api.datafy.com/` does return `strict-transport-security: max-age=15552000; includeSubDomains`. The host also returns a full Helmet-style header set (CSP, X-Content-Type-Options, X-Frame-Options, Referrer-Policy, COOP/CORP) behind Cloudflare, with Access-Control-Allow-Origin: *.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datafy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datafy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datafy
provider_slug: datafy
slug: datafy-domain-security
source_filename: datafy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:18:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.datafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:18:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: >-\n    Corrected by hand on 2026-08-12 from a direct probe. The automated pass\n    recorded hsts: null because every request to this host returns HTTP 500\n    (UnauthorizedError) and the header was not read off a non-2xx response;\n    `curl -I https://api.datafy.com/` does return\n    `strict-transport-security: max-age=15552000; includeSubDomains`. The host\n    also returns a full Helmet-style header set (CSP, X-Content-Type-Options,\n    X-Frame-Options, Referrer-Policy, COOP/CORP) behind Cloudflare, with\n    Access-Control-Allow-Origin:\
  \ *.\ndomains:\n- domain: datafy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafy/refs/heads/main/security/datafy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Advertising
- Location Intelligence
- Attribution
- Tourism
- Marketing
- Visitation Data
- Destination Marketing
- Measurement
---
