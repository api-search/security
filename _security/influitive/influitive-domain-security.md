---
api_specs:
- filename: influitive-events-openapi.json
  format: json
  label: Influitive Events API
  slug: influitive-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influitive/refs/heads/main/openapi/influitive-events-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: influitive.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 26 20:20:05 2026 GMT
  host: influitive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: influitive.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 13:07:50 2026 GMT
  host: api.influitive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Influitive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Influitive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Influitive
provider_slug: influitive
slug: influitive-domain-security
source_filename: influitive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: influitive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:20:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: influitive.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.influitive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:07:50 2026 GMT\n  hsts: null\ndomains:\n- domain: influitive.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influitive/refs/heads/main/security/influitive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Advocacy
- Customer Community
- Customer Engagement
- Advocacy Marketing
- Referral Marketing
- Customer Loyalty
- Gamification
- Webhooks
- SaaS
---
