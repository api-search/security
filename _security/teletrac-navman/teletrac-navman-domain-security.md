---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teletracnavman.com
  spf: true
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: www.teletracnavman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teletrac Navman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teletrac Navman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teletrac Navman
provider_slug: teletrac-navman
slug: teletrac-navman-domain-security
source_filename: teletrac-navman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teletracnavman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: teletracnavman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teletrac-navman/refs/heads/main/security/teletrac-navman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Driver Safety
- Compliance
- Company
---
