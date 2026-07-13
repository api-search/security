---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: invisionapp.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.invisionapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: support.invisionapp.com
  https: false
- host: projects.invisionapp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Invision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InVision, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: InVision
provider_slug: invision
slug: invision-domain-security
source_filename: invision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.invisionapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.invisionapp.com\n  https: false\n- host: projects.invisionapp.com\n  https: false\ndomains:\n- domain: invisionapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invision/refs/heads/main/security/invision-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Design
- Prototyping
- Design Systems
- Collaboration
- Digital Product Design
- Deprecated
---
