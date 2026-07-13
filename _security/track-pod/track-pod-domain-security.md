---
api_specs:
- filename: track-pod-openapi.yml
  format: yaml
  label: Track-POD API
  slug: track-pod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/openapi/track-pod-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: track-pod.com
  spf: true
hosts:
- cert_expires: Sep 10 06:46:21 2026 GMT
  host: www.track-pod.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.track-pod.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Track Pod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Track-POD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Track-POD
provider_slug: track-pod
slug: track-pod-domain-security
source_filename: track-pod-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.track-pod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:46:21 2026 GMT\n  hsts: false\n- host: api.track-pod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: track-pod.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/track-pod/refs/heads/main/security/track-pod-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Delivery
- Last Mile
- Logistics
- Proof Of Delivery
- Electronic Proof Of Delivery
- EPOD
- Route Planning
- Route Optimization
- Dispatch
- Fleet Management
- Driver Tracking
- Courier
- Field Service
- Transportation
- Shipping
---
