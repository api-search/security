---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omaticsoftware.com
  spf: true
hosts:
- cert_expires: Jan  1 22:32:01 2027 GMT
  host: omaticsoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Omaticsoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omatic Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Omatic Software
provider_slug: omaticsoftware
slug: omaticsoftware-domain-security
source_filename: omaticsoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omaticsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:32:01 2027 GMT\n  hsts: false\ndomains:\n- domain: omaticsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/omaticsoftware/security/omaticsoftware-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nonprofit
- Data Integration
- Cloud Platform
- Automation
- CRM
---
