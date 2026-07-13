---
api_specs:
- filename: usercentrics-app-cmp-sdk-openapi.yml
  format: yaml
  label: Usercentrics App CMP SDK
  slug: app-cmp-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-app-cmp-sdk-openapi.yml
- filename: usercentrics-web-cmp-v3-openapi.yml
  format: yaml
  label: Usercentrics Web CMP (V3)
  slug: web-cmp-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-web-cmp-v3-openapi.yml
- filename: usercentrics-cookiebot-cmp-openapi.yml
  format: yaml
  label: Cookiebot CMP
  slug: cookiebot-cmp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-cookiebot-cmp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usercentrics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cookiebot.com
  spf: true
hosts:
- cert_expires: Sep 15 05:37:49 2026 GMT
  host: usercentrics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:39:31 2026 GMT
  host: docs.usercentrics.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:05:53 2026 GMT
  host: www.cookiebot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usercentrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usercentrics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Usercentrics
provider_slug: usercentrics
slug: usercentrics-domain-security
source_filename: usercentrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usercentrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.usercentrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:39:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: www.cookiebot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:05:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usercentrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cookiebot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/security/usercentrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Privacy
- Consent
- CMP
- Compliance
- GDPR
- CCPA
- TCF
- GPP
- Cookies
- AI Governance
---
