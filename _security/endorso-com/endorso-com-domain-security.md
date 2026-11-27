---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endorso.com
  spf: true
hosts:
- cert_expires: Dec 19 13:33:57 2026 GMT
  host: endorso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Endorso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endorso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Endorso
provider_slug: endorso-com
slug: endorso-com-domain-security
source_filename: endorso-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endorso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 13:33:57 2026 GMT\n  hsts: false\ndomains:\n- domain: endorso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/endorso-com/security/endorso-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Affiliates
- E-Commerce
- Marketing
- Commissions
- Platform
---
