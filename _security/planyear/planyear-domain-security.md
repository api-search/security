---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: planyear.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: planyear.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Planyear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanYear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PlanYear
provider_slug: planyear
slug: planyear-domain-security
source_filename: planyear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planyear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: planyear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/planyear/security/planyear-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Benefits
- Insurance
- Platform
- Consulting
---
