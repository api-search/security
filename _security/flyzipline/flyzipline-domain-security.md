---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: flyzipline.com
  spf: true
hosts:
- cert_expires: Oct 14 21:10:09 2026 GMT
  host: flyzipline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flyzipline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flyzipline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flyzipline
provider_slug: flyzipline
slug: flyzipline-domain-security
source_filename: flyzipline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyzipline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:10:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flyzipline.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flyzipline/refs/heads/main/security/flyzipline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Drone Delivery
- Logistics
- Autonomous Systems
- Healthcare
- Robotics
- Last Mile Delivery
- Instant Logistics
---
