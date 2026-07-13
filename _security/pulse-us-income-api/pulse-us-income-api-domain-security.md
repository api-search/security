---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: webflow.io
  spf: false
hosts:
- cert_expires: Aug 25 03:06:04 2026 GMT
  host: pulseapi.webflow.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Us Income Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse US Income API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pulse US Income API
provider_slug: pulse-us-income-api
slug: pulse-us-income-api-domain-security
source_filename: pulse-us-income-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulseapi.webflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 03:06:04 2026 GMT\n  hsts: false\ndomains:\n- domain: webflow.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-us-income-api/refs/heads/main/security/pulse-us-income-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Income
- Underwriting
- Financial
- Applicants
---
