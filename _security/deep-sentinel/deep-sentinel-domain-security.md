---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deepsentinel.com
  spf: true
hosts:
- cert_expires: Sep 25 21:29:37 2026 GMT
  host: www.deepsentinel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 15:06:33 2026 GMT
  host: shop.deepsentinel.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deep Sentinel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Sentinel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Deep Sentinel
provider_slug: deep-sentinel
slug: deep-sentinel-domain-security
source_filename: deep-sentinel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepsentinel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:29:37 2026 GMT\n  hsts: false\n- host: shop.deepsentinel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:06:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: deepsentinel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-sentinel/refs/heads/main/security/deep-sentinel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Physical Security
- Video Surveillance
- Home Security
- Artificial Intelligence
- Computer-Vision
- Monitoring
- Internet of Things
- Commerce
---
