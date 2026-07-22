---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fanzapp.io
  spf: true
hosts:
- cert_expires: Oct 18 07:48:06 2026 GMT
  host: fanzapp.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamup Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamUp Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TeamUp Inc.
provider_slug: teamup-inc
slug: teamup-inc-domain-security
source_filename: teamup-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fanzapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:48:06 2026 GMT\n  hsts: false\ndomains:\n- domain: fanzapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamup-inc/refs/heads/main/security/teamup-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Sports
- Football
- Fan Engagement
- Fantasy Sports
- Gaming
- Mobile
- Consumer
---
