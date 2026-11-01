---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: samdesk.nl
  spf: true
hosts:
- cert_expires: Jan  1 21:48:56 2027 GMT
  host: samdesk.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Samdesk Nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for samdesk-nl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: samdesk-nl
provider_slug: samdesk-nl
slug: samdesk-nl-domain-security
source_filename: samdesk-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: samdesk.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 21:48:56 2027 GMT\n  hsts: false\ndomains:\n- domain: samdesk.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/samdesk-nl/security/samdesk-nl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CRM
- Helpdesk
- E-commerce
- AI
---
