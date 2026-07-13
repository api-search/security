---
api_specs:
- filename: docs
  format: yaml
  label: Rockerbox API
  slug: rockerbox-api
  spec_type: OpenAPI
  url: https://backend-prod-k8s.rockerbox.tech/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rockerbox.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rockerbox.tech
  spf: true
hosts:
- cert_expires: Sep 28 17:02:06 2026 GMT
  host: www.rockerbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 10:19:54 2026 GMT
  host: help.rockerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: backend-prod-k8s.rockerbox.tech
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rockerbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockerbox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rockerbox
provider_slug: rockerbox
slug: rockerbox-domain-security
source_filename: rockerbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.rockerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:19:54 2026 GMT\n  hsts: false\n- host: backend-prod-k8s.rockerbox.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rockerbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rockerbox.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockerbox/refs/heads/main/security/rockerbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Attribution
- Multi-Touch Attribution
- Marketing Mix Modeling
- Incrementality Testing
- Media Spend
- Customer Journeys
- Marketing Analytics
---
