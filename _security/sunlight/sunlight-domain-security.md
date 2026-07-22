---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sunlight.is
  spf: true
hosts:
- host: sunlight.is
  https: false
- cert_expires: Sep 30 05:56:19 2026 GMT
  host: docs.sunlight.is
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: app.sunlight.is
  https: false
kind: domain-security
layout: security
method: probed
name: Sunlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunlight, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sunlight
provider_slug: sunlight
slug: sunlight-domain-security
source_filename: sunlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunlight.is\n  https: false\n- host: docs.sunlight.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:56:19 2026 GMT\n  hsts: false\n- host: app.sunlight.is\n  https: false\ndomains:\n- domain: sunlight.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunlight/refs/heads/main/security/sunlight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Learning
- Budgeting
- Spending
- Fintech
- JSON:API
- Groups
- Orders
---
