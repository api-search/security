---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hull.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hullapp.io
  spf: true
hosts:
- host: www.hull.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.hull.io'
- host: hullapp.io
  https: false
kind: domain-security
layout: security
method: probed
name: Hull Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hull, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hull
provider_slug: hull
slug: hull-domain-security
source_filename: hull-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hull.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.hull.io'\n  hsts: null\n- host: hullapp.io\n  https: false\ndomains:\n- domain: hull.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hullapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hull/refs/heads/main/security/hull-domain-security.yml
summary_line: DMARC
tags:
- Company
- Customer Data Platform
- CDP
- Identity Resolution
- Data Integration
- Customer Data
- Marketing
- Real-Time
- iPaaS
- Analytics
---
