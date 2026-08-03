---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firehawkdefense.com
  spf: true
hosts:
- cert_expires: Sep 14 22:47:43 2026 GMT
  host: firehawkdefense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firehawk Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firehawk Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Firehawk Aerospace
provider_slug: firehawk-aerospace
slug: firehawk-aerospace-domain-security
source_filename: firehawk-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firehawkdefense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:47:43 2026 GMT\n  hsts: false\ndomains:\n- domain: firehawkdefense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehawk-aerospace/refs/heads/main/security/firehawk-aerospace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Defense
- Rocket Propulsion
- Additive Manufacturing
- Energetics
- Manufacturing
- Space
- Texas
---
