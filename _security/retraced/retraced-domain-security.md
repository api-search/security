---
api_specs:
- filename: retraced-openapi-original.json
  format: json
  label: Retraced Public API
  slug: retraced-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: retraced.com
  spf: true
hosts:
- cert_expires: Sep 15 12:48:34 2026 GMT
  host: www.retraced.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 00:23:43 2026 GMT
  host: publicapi.retraced.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retraced Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retraced, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Retraced
provider_slug: retraced
slug: retraced-domain-security
source_filename: retraced-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.retraced.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:48:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: publicapi.retraced.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: retraced.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/security/retraced-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Applicative Saas
- Supply Chain
- Sustainability
- Compliance
- Fashion
- Traceability
- Digital Product Passport
- ESG
---
