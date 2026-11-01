---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: interaction.co
  spf: true
hosts:
- cert_expires: Jan  9 15:21:27 2027 GMT
  host: interaction.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Interaction Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Interaction Company Of California, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Interaction Company Of California
provider_slug: interaction-co
slug: interaction-co-domain-security
source_filename: interaction-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interaction.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 15:21:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: interaction.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/interaction-co/security/interaction-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Platform
- Developer
- Interaction
---
