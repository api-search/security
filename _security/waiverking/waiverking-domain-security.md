---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: waiverking.com
  spf: true
hosts:
- cert_expires: Feb 14 07:32:51 2027 GMT
  host: waiverking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WaiverKing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WaiverKing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WaiverKing
provider_slug: waiverking
slug: waiverking-domain-security
source_filename: waiverking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waiverking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 07:32:51 2027 GMT\n  hsts: false\ndomains:\n- domain: waiverking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/waiverking/security/waiverking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software-as-a-Service
- Fitness
- Wellness
- Digital Forms
- Waiver
---
