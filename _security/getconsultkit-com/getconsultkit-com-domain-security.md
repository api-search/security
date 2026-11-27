---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getconsultkit.com
  spf: true
hosts:
- cert_expires: Dec 23 15:00:13 2026 GMT
  host: getconsultkit.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConsultKit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConsultKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConsultKit
provider_slug: getconsultkit-com
slug: getconsultkit-com-domain-security
source_filename: getconsultkit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getconsultkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 15:00:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: getconsultkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getconsultkit-com/security/getconsultkit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consulting
- Productivity
- Referrals
- Software-as-a-Service
- Platform
---
