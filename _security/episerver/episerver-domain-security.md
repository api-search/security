---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: episerver.com
  spf: true
hosts:
- cert_expires: Aug  1 07:53:06 2026 GMT
  host: www.episerver.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Episerver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Episerver, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Episerver
provider_slug: episerver
slug: episerver-domain-security
source_filename: episerver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.episerver.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  1 07:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: episerver.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/episerver/refs/heads/main/security/episerver-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Enterprise
- Content Management
- Digital Experience Platform
- CMS
- Commerce
- Experimentation
- Personalization
- GraphQL
- SDKs
---
