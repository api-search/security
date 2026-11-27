---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getboothiq.com
  spf: true
hosts:
- cert_expires: Feb  6 07:21:10 2027 GMT
  host: getboothiq.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BoothIQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoothIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BoothIQ
provider_slug: getboothiq-com
slug: getboothiq-com-domain-security
source_filename: getboothiq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getboothiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 07:21:10 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: getboothiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getboothiq-com/security/getboothiq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Capture
- Trade Shows
- Artificial Intelligence
- CRM Integration
- Offline Capture
---
