---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alchemynano.com
  spf: true
hosts:
- cert_expires: Dec 12 16:54:37 2026 GMT
  host: www.alchemynano.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alchemynano Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alchemy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alchemy
provider_slug: alchemynano-com
slug: alchemynano-com-domain-security
source_filename: alchemynano-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alchemynano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:54:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alchemynano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/alchemynano-com/security/alchemynano-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nanocoatings
- Automotive
- Defence
---
