---
api_specs:
- filename: konfetti-store-openapi.yml
  format: yaml
  label: konfetti Store API
  slug: store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-store-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gokonfetti.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: gokonfetti.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: backoffice.gokonfetti.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api.gokonfetti.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Konfetti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for konfetti, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: konfetti
provider_slug: konfetti
slug: konfetti-domain-security
source_filename: konfetti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gokonfetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: backoffice.gokonfetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.gokonfetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gokonfetti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/security/konfetti-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Experiences
- Booking
- Events
- Workshops
- Ticketing
- Gift Cards
- Travel and Leisure
- Germany
- Commerce
---
