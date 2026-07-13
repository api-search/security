---
api_specs:
- filename: ourpeople-openapi.yml
  format: yaml
  label: OurPeople API
  slug: ourpeople-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/openapi/ourpeople-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ourpeople.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ourpeople.co
  spf: true
hosts:
- cert_expires: Sep 17 14:11:49 2026 GMT
  host: developer.ourpeople.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 18:08:53 2026 GMT
  host: ourpeople.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: example-api.ourpeople.co
  https: false
kind: domain-security
layout: security
method: probed
name: Ourpeople Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OurPeople, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OurPeople
provider_slug: ourpeople
slug: ourpeople-domain-security
source_filename: ourpeople-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ourpeople.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:11:49 2026 GMT\n  hsts: false\n- host: ourpeople.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:08:53 2026 GMT\n  hsts: false\n- host: example-api.ourpeople.co\n  https: false\ndomains:\n- domain: ourpeople.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ourpeople.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/security/ourpeople-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Communications
- Workforce
- Frontline
---
