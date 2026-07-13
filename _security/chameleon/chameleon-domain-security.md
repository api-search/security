---
api_specs:
- filename: chameleon-openapi.yml
  format: yaml
  label: Chameleon REST API
  slug: chameleon-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 iodef "mailto:caa-reports@chameleon.io"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chameleon.io
  spf: true
hosts:
- cert_expires: Sep 15 04:33:16 2026 GMT
  host: www.chameleon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 00:30:25 2026 GMT
  host: developers.chameleon.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 20:33:06 2026 GMT
  host: api.chameleon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chameleon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chameleon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chameleon
provider_slug: chameleon
slug: chameleon-domain-security
source_filename: chameleon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chameleon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:33:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.chameleon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chameleon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:33:06 2026 GMT\n  hsts: null\ndomains:\n- domain: chameleon.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 iodef \"mailto:caa-reports@chameleon.io\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/security/chameleon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product
- In-App Guidance
- Onboarding
- Surveys
- Analytics
---
