---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fly.dev
  spf: false
hosts:
- cert_expires: Nov 19 11:49:32 2026 GMT
  host: payload-rail.fly.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Revrule Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RevRule by Payload, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RevRule by Payload
provider_slug: revrule
slug: revrule-domain-security
source_filename: revrule-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payload-rail.fly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:49:32 2026 GMT\n  hsts: null\ndomains:\n- domain: fly.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revrule/refs/heads/main/security/revrule-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Revenue
- Payments
- Fintech
---
