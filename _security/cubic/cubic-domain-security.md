---
api_specs:
- filename: cubic-umo-iq-public-feed-openapi.yml
  format: yaml
  label: Umo IQ Public Feed API
  slug: umo-iq-public-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubic/refs/heads/main/openapi/cubic-umo-iq-public-feed-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cubic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umoiq.com
  spf: true
hosts:
- cert_expires: Nov 22 07:58:22 2026 GMT
  host: www.cubic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: retro.umoiq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cubic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cubic
provider_slug: cubic
slug: cubic-domain-security
source_filename: cubic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:58:22 2026 GMT\n  hsts: false\n- host: retro.umoiq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cubic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: umoiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubic/refs/heads/main/security/cubic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Transportation
- Technology
- Public Transit
- Fare Collection
- Real-Time Data
- Vehicle Location
- Intelligent Transportation Systems
---
