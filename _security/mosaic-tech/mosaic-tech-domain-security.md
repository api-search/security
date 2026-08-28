---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mosaic.tech
  spf: true
hosts:
- cert_expires: Oct 10 11:39:28 2026 GMT
  host: www.mosaic.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosaic Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosaic Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mosaic Tech
provider_slug: mosaic-tech
slug: mosaic-tech-domain-security
source_filename: mosaic-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mosaic.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:39:28 2026 GMT\n  hsts: null\ndomains:\n- domain: mosaic.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaic-tech/refs/heads/main/security/mosaic-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Planning
- FP&A
- Strategic Finance
- Business Intelligence
- Analytics
- SaaS
- Acquired
---
