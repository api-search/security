---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cannonvoip.com
  spf: true
hosts:
- cert_expires: Jan 29 09:03:07 2027 GMT
  host: cannonvoip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cannon VoIP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cannon VoIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cannon VoIP
provider_slug: cannonvoip-com
slug: cannonvoip-com-domain-security
source_filename: cannonvoip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cannonvoip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 09:03:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cannonvoip.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cannonvoip-com/security/cannonvoip-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- VoIP
- Business Communications
- Cloud Phone System
- US
- Software-as-a-Service
---
