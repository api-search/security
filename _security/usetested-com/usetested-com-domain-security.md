---
api_specs:
- filename: usetested-com-directory-api-openapi.yml
  format: yaml
  label: UseTested Directory API
  slug: usetested-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetested-com/openapi/usetested-com-directory-api-openapi.yml
- filename: usetested-com-paid-api-openapi.yml
  format: yaml
  label: UseTested Paid API
  slug: usetested-com-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetested-com/openapi/usetested-com-paid-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usetested.com
  spf: false
hosts:
- cert_expires: Feb 19 09:30:13 2027 GMT
  host: usetested.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: UseTested Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UseTested, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: UseTested
provider_slug: usetested-com
slug: usetested-com-domain-security
source_filename: usetested-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetested.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 09:30:13 2027 GMT\n  hsts: false\ndomains:\n- domain: usetested.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usetested-com/security/usetested-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Directory
- API
- Testing
- On‑chain
- Agent Services
- Machine Payments
---
