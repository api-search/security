---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lichidare.md
  spf: true
hosts:
- cert_expires: Feb 12 03:30:14 2027 GMT
  host: lichidare.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lichidare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lichidare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lichidare
provider_slug: lichidare-md
slug: lichidare-md-domain-security
source_filename: lichidare-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lichidare.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 03:30:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lichidare.md\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lichidare-md/security/lichidare-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Auctions
- Insolvency
- Moldova
- Real Estate
- Transport
---
