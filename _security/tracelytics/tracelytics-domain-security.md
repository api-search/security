---
description: ''
domains:
- a_records: false
  caa: []
  dmarc: false
  dnssec: false
  domain: tracelytics.com
  ns_records: false
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appneta.com
  spf: true
hosts:
- host: tracelytics.com
  https: false
  resolves: false
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: appneta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tracelytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tracelytics, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tracelytics
provider_slug: tracelytics
slug: tracelytics-domain-security
source_filename: tracelytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes: >-\n  appneta.com is the domain of Tracelytics's 2012 acquirer AppNeta (itself now\n  redirecting to broadcom.com/appneta). The company's own domain tracelytics.com\n  is dead — probed 2026-07-21 with no A or NS records and no HTTPS connection —\n  recorded below as valid absence data.\nhosts:\n- host: tracelytics.com\n  https: false\n  resolves: false\n- host: appneta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tracelytics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  a_records: false\n  ns_records: false\n- domain: appneta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracelytics/refs/heads/main/security/tracelytics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Application Performance Monitoring
- Tracing
- Observability
- Acquired
---
