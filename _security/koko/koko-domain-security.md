---
api_specs:
- filename: koko-countries-api-openapi.yml
  format: yaml
  label: Koko Countries API
  slug: koko-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koko/refs/heads/main/openapi/koko-countries-api-openapi.yml
- filename: koko-helplines-api-openapi.yml
  format: yaml
  label: Koko Helplines API
  slug: koko-helplines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koko/refs/heads/main/openapi/koko-helplines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kokocares.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: koko.ai
  spf: false
hosts:
- cert_expires: Oct  8 19:32:50 2026 GMT
  host: kokocares.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:25:19 2026 GMT
  host: developers.kokocares.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 18:31:24 2026 GMT
  host: helpline-api.koko.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koko, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Koko
provider_slug: koko
slug: koko-domain-security
source_filename: koko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kokocares.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.kokocares.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: helpline-api.koko.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 18:31:24 2026 GMT\n  hsts: false\ndomains:\n- domain: kokocares.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: koko.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koko/refs/heads/main/security/koko-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mental Health
- Crisis Support
- Suicide Prevention
- Trust and Safety
- Content Moderation
- Nonprofit
- Health
- Helplines
---
