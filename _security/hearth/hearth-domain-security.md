---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gethearth.com
  spf: true
hosts:
- cert_expires: Oct 14 05:32:35 2026 GMT
  host: gethearth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hearth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hearth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hearth
provider_slug: hearth
slug: hearth-domain-security
source_filename: hearth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gethearth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:32:35 2026 GMT\n  hsts: false\ndomains:\n- domain: gethearth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hearth/refs/heads/main/security/hearth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contractors
- Home Improvement
- Financing
- Payments
- Invoicing
- Scheduling
- Field Service
- AI Assistant
- SaaS
---
