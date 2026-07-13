---
api_specs:
- filename: punchh-mobile-openapi.yml
  format: yaml
  label: PAR Punchh Mobile API
  slug: mobile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-openapi.yml
- filename: punchh-online-ordering-openapi.yml
  format: yaml
  label: PAR Punchh Online Ordering and SSO API
  slug: online-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-openapi.yml
- filename: punchh-pos-openapi.yml
  format: yaml
  label: PAR Punchh POS and Kiosk API
  slug: pos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-openapi.yml
- filename: punchh-platform-functions-openapi.yml
  format: yaml
  label: PAR Punchh Platform Functions API
  slug: platform-functions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: punchh.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partech.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: punchh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:18:33 2026 GMT
  host: developers.partech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Punchh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Punchh, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Punchh
provider_slug: punchh
slug: punchh-domain-security
source_filename: punchh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: punchh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: developers.partech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:18:33 2026 GMT\n  hsts: false\ndomains:\n- domain: punchh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: partech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/security/punchh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Loyalty
- Marketing
- Guest Engagement
- Online Ordering
- Mobile
- Point Of Sale
- Webhooks
---
