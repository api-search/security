---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uberfreight.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uber.com
  spf: true
hosts:
- cert_expires: Oct  7 21:39:46 2026 GMT
  host: www.uberfreight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: developer.uberfreight.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uber Freight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uber Freight, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Uber Freight
provider_slug: uber-freight
slug: uber-freight-domain-security
source_filename: uber-freight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uberfreight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.uberfreight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\n- host: api.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: uberfreight.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-freight/refs/heads/main/security/uber-freight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Freight
- Logistics
- Trucking
- Shipping
- Transportation
- Supply Chain
- Truckload
- Carrier Network
- TMS
- Digital Freight Broker
---
