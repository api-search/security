---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: federatedwireless.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: federatedwireless.com
  spf: true
hosts:
- cert_expires: Nov  8 04:15:10 2026 GMT
  host: federatedwireless.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 13:38:42 2026 GMT
  host: myfederated.federatedwireless.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federated Wireless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federated Wireless, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Federated Wireless
provider_slug: federated-wireless
slug: federated-wireless-domain-security
source_filename: federated-wireless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: federatedwireless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 04:15:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myfederated.federatedwireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:38:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: federatedwireless.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: federatedwireless.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federated-wireless/refs/heads/main/security/federated-wireless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Spectrum
- CBRS
- Wireless
- Telecommunications
- Private 5G
- Shared Spectrum
- Spectrum Access System
- 6 GHz
- Network Planning
- RF Engineering
- Government
---
