---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: isoligne.com
  spf: true
hosts:
- cert_expires: Jan  9 02:03:25 2027 GMT
  host: isoligne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Isoligne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Isoligne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Isoligne
provider_slug: isoligne-com
slug: isoligne-com-domain-security
source_filename: isoligne-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isoligne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 02:03:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: isoligne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/isoligne-com/security/isoligne-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Customer Experience
- Software-as-a-Service
- Automation
- French
---
