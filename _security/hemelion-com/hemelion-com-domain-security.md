---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hemelion.com
  spf: true
hosts:
- cert_expires: Dec 21 10:43:48 2026 GMT
  host: hemelion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hemelion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hemelion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hemelion
provider_slug: hemelion-com
slug: hemelion-com-domain-security
source_filename: hemelion-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hemelion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 10:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hemelion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hemelion-com/security/hemelion-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing
- Platform
- Decision-Making
- Product Development
- Software-as-a-Service
---
