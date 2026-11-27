---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leadquasar.com
  spf: true
hosts:
- cert_expires: Feb 13 03:14:54 2027 GMT
  host: leadquasar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Answerflix Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Answerflix Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Answerflix Ltd
provider_slug: leadquasar-com
slug: leadquasar-com-domain-security
source_filename: leadquasar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadquasar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 03:14:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leadquasar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/leadquasar-com/security/leadquasar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Lead Generation
- Artificial Intelligence
- Marketing
- Data
---
