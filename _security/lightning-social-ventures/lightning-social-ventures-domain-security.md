---
api_specs:
- filename: lightning-social-ventures-lightning-reach-openapi.json
  format: json
  label: Lightning Reach API
  slug: lightning-reach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/openapi/lightning-social-ventures-lightning-reach-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lightningreach.org
  spf: true
hosts:
- cert_expires: Sep 16 10:56:30 2026 GMT
  host: lightningreach.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 11:25:06 2026 GMT
  host: api.lightningreach.org
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'The automated HEAD probe recorded hsts as null because the host answers 401 to unauthenticated requests. A direct GET on 2026-07-19 returned ''strict-transport-security: max-age=31536000; includeSubDomains'' alongside a full Helmet header set (CSP, X-Content-Type-Options, X-Frame-Options, Referrer-Policy, COOP, CORP). Corrected by hand from that observation.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightning Social Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightning Social Ventures, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lightning Social Ventures
provider_slug: lightning-social-ventures
slug: lightning-social-ventures-domain-security
source_filename: lightning-social-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightningreach.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:56:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.lightningreach.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The automated HEAD probe recorded hsts as null because the host answers 401\n    to unauthenticated requests. A direct GET on 2026-07-19 returned\n    'strict-transport-security: max-age=31536000; includeSubDomains' alongside a\n    full Helmet header set (CSP, X-Content-Type-Options, X-Frame-Options,\n    Referrer-Policy, COOP, CORP). Corrected by hand from that observation.\ndomains:\n- domain: lightningreach.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/security/lightning-social-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Inclusion
- Grants
- Social Impact
- Nonprofit
- Housing
- Government
- Welfare Benefits
- United Kingdom
---
