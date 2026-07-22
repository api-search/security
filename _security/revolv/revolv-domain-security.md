---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revolv.com
  spf: true
hosts:
- cert_expires: Sep 21 08:38:00 2026 GMT
  host: revolv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revolv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revolv
provider_slug: revolv
slug: revolv-domain-security
source_filename: revolv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revolv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:38:00 2026 GMT\n  hsts: false\ndomains:\n- domain: revolv.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolv/refs/heads/main/security/revolv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Smart Home
- Internet of Things
- Home Automation
- Consumer Electronics
- Connected Devices
- Defunct
---
