---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eventnoire.com
  spf: true
hosts:
- cert_expires: Aug 14 23:18:40 2026 GMT
  host: eventnoire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventnoire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventnoire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eventnoire
provider_slug: eventnoire
slug: eventnoire-domain-security
source_filename: eventnoire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventnoire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:18:40 2026 GMT\n  hsts: false\ndomains:\n- domain: eventnoire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventnoire/refs/heads/main/security/eventnoire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Events
- Ticketing
- Event Discovery
- Event Management
- Culture
- Consumer
---
