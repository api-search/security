---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amphiform.com
  spf: true
hosts:
- cert_expires: Sep 21 10:56:13 2026 GMT
  host: amphiform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amphiform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amphiform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amphiform
provider_slug: amphiform
slug: amphiform-domain-security
source_filename: amphiform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amphiform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:56:13 2026 GMT\n  hsts: false\ndomains:\n- domain: amphiform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amphiform/refs/heads/main/security/amphiform-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy Infrastructure
- Energy
- Clean Energy
- Materials Science
- Manufacturing
- Deep Tech
- Decarbonization
---
