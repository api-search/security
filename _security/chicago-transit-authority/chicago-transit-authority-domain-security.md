---
api_specs:
- filename: cta-train-tracker-openapi.yml
  format: yaml
  label: CTA Train Tracker API
  slug: train-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/cta-train-tracker-openapi.yml
- filename: cta-bus-tracker-openapi.yml
  format: yaml
  label: CTA Bus Tracker API
  slug: bus-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/cta-bus-tracker-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transitchicago.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ctabustracker.com
  spf: false
hosts:
- cert_expires: Sep 14 17:15:30 2026 GMT
  host: www.transitchicago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:02:11 2026 GMT
  host: lapi.transitchicago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: www.ctabustracker.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chicago Transit Authority Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chicago Transit Authority, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chicago Transit Authority
provider_slug: chicago-transit-authority
slug: chicago-transit-authority-domain-security
source_filename: chicago-transit-authority-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transitchicago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:15:30 2026 GMT\n  hsts: null\n- host: lapi.transitchicago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:02:11 2026 GMT\n  hsts: null\n- host: www.ctabustracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: transitchicago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ctabustracker.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/security/chicago-transit-authority-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Bus
- Bus Tracker
- Chicago
- CTA
- Customer Alerts
- GTFS
- L Train
- Open Data
- Public Transit
- Real-Time
- Train
- Train Tracker
- Transit
- Transportation
---
