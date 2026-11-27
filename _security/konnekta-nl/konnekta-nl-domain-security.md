---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konnekta.nl
  spf: false
hosts:
- cert_expires: Feb  9 09:54:02 2027 GMT
  host: konnekta.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Konnekta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konnekta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Konnekta
provider_slug: konnekta-nl
slug: konnekta-nl-domain-security
source_filename: konnekta-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konnekta.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 09:54:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: konnekta.nl\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/konnekta-nl/security/konnekta-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Integration
- Accounting
- Dutch
- Small Business
---
