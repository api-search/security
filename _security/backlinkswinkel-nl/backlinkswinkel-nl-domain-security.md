---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backlinkswinkel.nl
  spf: false
hosts:
- cert_expires: Jan 26 12:11:52 2027 GMT
  host: backlinkswinkel.nl
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BacklinksWinkel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BacklinksWinkel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BacklinksWinkel
provider_slug: backlinkswinkel-nl
slug: backlinkswinkel-nl-domain-security
source_filename: backlinkswinkel-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backlinkswinkel.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 12:11:52 2027 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: backlinkswinkel.nl\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/backlinkswinkel-nl/security/backlinkswinkel-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Link Building
- Backlinks
- Dutch
- Marketing
---
