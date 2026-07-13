---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 1 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: rockwellautomation.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plex.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.rockwellautomation.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: developers.plex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: plex.rockwellautomation.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rockwell Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockwell Automation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rockwell Automation
provider_slug: rockwell-automation
slug: rockwell-automation-domain-security
source_filename: rockwell-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockwellautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.plex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plex.rockwellautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rockwellautomation.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 1 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: plex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-automation/refs/heads/main/security/rockwell-automation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial Automation
- Manufacturing
- PLC
- SCADA
- IIoT
- Fortune 500
---
