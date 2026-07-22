---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beaubble.com
  spf: true
hosts:
- cert_expires: Oct 16 03:50:18 2026 GMT
  host: beaubble.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beaubble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beaubble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beaubble
provider_slug: beaubble
slug: beaubble-domain-security
source_filename: beaubble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beaubble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:50:18 2026 GMT\n  hsts: false\ndomains:\n- domain: beaubble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaubble/refs/heads/main/security/beaubble-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Beauty
- Cosmetics
- Ecommerce
- Creator Economy
- Direct-to-Consumer
- Consumer
---
