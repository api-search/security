---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fermat360.nl
  spf: true
hosts:
- cert_expires: Dec 29 11:54:18 2026 GMT
  host: fermat360.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fermat 360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fermat 360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fermat 360
provider_slug: fermat360-nl
slug: fermat360-nl-domain-security
source_filename: fermat360-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fermat360.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 11:54:18 2026 GMT\n  hsts: false\ndomains:\n- domain: fermat360.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fermat360-nl/security/fermat360-nl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Legal Tech
- Artificial Intelligence
- Search
- Netherlands
- Software-as-a-Service
---
