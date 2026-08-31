---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: headlight.health
  spf: true
hosts:
- cert_expires: Sep 16 00:28:10 2026 GMT
  host: headlight.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Headlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Headlight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Headlight
provider_slug: headlight
slug: headlight-domain-security
source_filename: headlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headlight.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:28:10 2026 GMT\n  hsts: false\ndomains:\n- domain: headlight.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headlight/refs/heads/main/security/headlight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthtech
- Mental Health
- Telehealth
- Teletherapy
- Psychiatry
- Behavioral Health
- Healthcare
---
