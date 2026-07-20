---
api_specs:
- filename: bluecore-openapi.yml
  format: yaml
  label: Bluecore API
  slug: bluecore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bluecore.com
  spf: true
hosts:
- cert_expires: Sep 28 02:55:48 2026 GMT
  host: bluecore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 18:32:36 2026 GMT
  host: a.bluecore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluecore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluecore, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bluecore
provider_slug: bluecore
slug: bluecore-domain-security
source_filename: bluecore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:55:48 2026 GMT\n  hsts: false\n- host: a.bluecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:32:36 2026 GMT\n  hsts: null\ndomains:\n- domain: bluecore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/security/bluecore-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- eCommerce
- Consent
---
