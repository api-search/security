---
api_specs:
- filename: paper-instruments-openapi-generated.yml
  format: yaml
  label: Paper Instruments API
  slug: paper-instruments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paper-instruments/openapi/_ae-authored/paper-instruments-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paperinstruments.com
  spf: true
hosts:
- cert_expires: Nov 27 16:10:03 2026 GMT
  host: paperinstruments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paper Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paper Instruments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paper Instruments
provider_slug: paper-instruments
slug: paper-instruments-domain-security
source_filename: paper-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paperinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 16:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paperinstruments.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/paper-instruments/security/paper-instruments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Open-Source
- Finance
- Consulting
- Law
---
