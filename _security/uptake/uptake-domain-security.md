---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uptake.com
  spf: true
hosts:
- cert_expires: Sep 12 13:56:37 2026 GMT
  host: uptake.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 17:07:04 2026 GMT
  host: api.uptake.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uptake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uptake, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Uptake
provider_slug: uptake
slug: uptake-domain-security
source_filename: uptake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:56:37 2026 GMT\n  hsts: false\n- host: api.uptake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 17:07:04 2026 GMT\n  hsts: null\ndomains:\n- domain: uptake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptake/refs/heads/main/security/uptake-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial AI
- Predictive Maintenance
- Asset Performance Management
- Fleet Management
- Telematics
- Machine Learning
- Industrial IoT
---
