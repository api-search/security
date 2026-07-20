---
api_specs:
- filename: headout-partner-openapi.yml
  format: yaml
  label: Headout Partner API
  slug: headout-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/headout/refs/heads/main/openapi/headout-partner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: headout.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: test-headout.com
  spf: false
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: headout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.headout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: sandbox.api.test-headout.com
  https: false
kind: domain-security
layout: security
method: probed
name: Headout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeadOut, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HeadOut
provider_slug: headout
slug: headout-domain-security
source_filename: headout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: www.headout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox.api.test-headout.com\n  https: false\ndomains:\n- domain: headout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: test-headout.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headout/refs/heads/main/security/headout-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Tours and Activities
- Experiences
- Attractions
- Ticketing
- Bookings
- Marketplace
- Partner API
- Affiliate
- Events
---
