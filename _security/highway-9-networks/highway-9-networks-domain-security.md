---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: highway9.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: highway9networks.com
  spf: true
hosts:
- cert_expires: Aug 19 15:39:48 2026 GMT
  host: highway9.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 09:12:02 2026 GMT
  host: partner.demo.highway9networks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highway 9 Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highway 9 Networks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Highway 9 Networks
provider_slug: highway-9-networks
slug: highway-9-networks-domain-security
source_filename: highway-9-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highway9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:39:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.demo.highway9networks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:12:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: highway9.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: highway9networks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highway-9-networks/refs/heads/main/security/highway-9-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- 5G
- Private Mobile Networks
- Enterprise Wireless
- Edge Computing
- Network Infrastructure
- IoT
- Deterministic Wireless
- Artificial Intelligence
---
