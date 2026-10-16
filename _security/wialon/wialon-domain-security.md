---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wialon.com
  spf: true
hosts:
- cert_expires: Feb  5 20:08:18 2027 GMT
  host: wialon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wialon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wialon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Wialon
provider_slug: wialon
slug: wialon-domain-security
source_filename: wialon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wialon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 20:08:18 2027 GMT\n  hsts: false\ndomains:\n- domain: wialon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wialon/refs/heads/main/security/wialon-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fleet Management
- Telematics
- GPS Tracking
- API
---
