---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartdrive.net
  spf: true
hosts:
- cert_expires: Jan  9 18:25:06 2027 GMT
  host: www.smartdrive.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smartdrive Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartDrive Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SmartDrive Systems
provider_slug: smartdrive-systems
slug: smartdrive-systems-domain-security
source_filename: smartdrive-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartdrive.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:25:06 2027 GMT\n  hsts: false\ndomains:\n- domain: smartdrive.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/smartdrive-systems/security/smartdrive-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Safety
- Transportation Intelligence
- Fleet Management
- Telematics
- Compliance
- Analytics
---
