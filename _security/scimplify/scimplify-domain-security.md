---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scimplify.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.scimplify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scimplify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scimplify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scimplify
provider_slug: scimplify
slug: scimplify-domain-security
source_filename: scimplify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scimplify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: scimplify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scimplify/refs/heads/main/security/scimplify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Chemicals
- Specialty Chemicals
- Manufacturing
- Pharmaceutical
- Agrochemicals
- Sourcing
- CRO
- CMO
---
