---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: electricskateboard.com
  spf: false
hosts:
- cert_expires: Jan 30 18:34:07 2027 GMT
  host: electricskateboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Electric Skateboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electric Skateboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Electric Skateboard
provider_slug: electricskateboard-com
slug: electricskateboard-com-domain-security
source_filename: electricskateboard-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: electricskateboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 18:34:07 2027 GMT\n  hsts: false\ndomains:\n- domain: electricskateboard.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/electricskateboard-com/security/electricskateboard-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Electric Skateboards
- Streetwear
- Pricing
---
