---
api_specs:
- filename: bidmachine-io-placement-management-openapi.yml
  format: yaml
  label: BidMachine Placement Management API
  slug: bidmachine-placement-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/openapi/bidmachine-io-placement-management-openapi.yml
- filename: bidmachine-io-reporting-openapi.yml
  format: yaml
  label: BidMachine Reporting API
  slug: bidmachine-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/openapi/bidmachine-io-reporting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bidmachine.io
  spf: true
hosts:
- cert_expires: Nov 15 08:31:30 2026 GMT
  host: bidmachine.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 14:23:09 2026 GMT
  host: developers.bidmachine.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api-eu.bidmachine.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bidmachine Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BidMachine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BidMachine
provider_slug: bidmachine-io
slug: bidmachine-io-domain-security
source_filename: bidmachine-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidmachine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 08:31:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.bidmachine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 14:23:09 2026 GMT\n  hsts: false\n- host: api-eu.bidmachine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bidmachine.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/security/bidmachine-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AdTech
- Mobile Advertising
- Ad Exchange
- Ad Mediation
- In-App Bidding
- OpenRTB
- App Monetization
- Programmatic Advertising
- Mobile SDK
- Reporting
- Company
---
