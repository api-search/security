---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: speakerdeck.com
  spf: true
hosts:
- cert_expires: Dec 18 20:30:21 2026 GMT
  host: speakerdeck.com
  hsts: true
  hsts_max_age: 15778476
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Speakerdeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speaker Deck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Speaker Deck
provider_slug: speakerdeck
slug: speakerdeck-domain-security
source_filename: speakerdeck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speakerdeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 20:30:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15778476\ndomains:\n- domain: speakerdeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/speakerdeck/security/speakerdeck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Presentation
- Sharing
- Slides
- Education
- Developer
---
