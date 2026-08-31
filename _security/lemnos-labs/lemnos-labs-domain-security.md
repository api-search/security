---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lemnos.vc
  spf: false
hosts:
- cert_expires: Sep 30 15:33:53 2026 GMT
  host: lemnos.vc
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemnos Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemnos Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lemnos Labs
provider_slug: lemnos-labs
slug: lemnos-labs-domain-security
source_filename: lemnos-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemnos.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: lemnos.vc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemnos-labs/refs/heads/main/security/lemnos-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Deeptech
- Hardware
- Robotics
- Seed Stage
- Investors
---
