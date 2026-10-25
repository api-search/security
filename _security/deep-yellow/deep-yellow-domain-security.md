---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepyellow.com.au
  spf: true
hosts:
- cert_expires: Nov 26 22:20:02 2026 GMT
  host: deepyellow.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deep Yellow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Yellow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deep Yellow
provider_slug: deep-yellow
slug: deep-yellow-domain-security
source_filename: deep-yellow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepyellow.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:20:02 2026 GMT\n  hsts: false\ndomains:\n- domain: deepyellow.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-yellow/refs/heads/main/security/deep-yellow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mining
- Uranium
- Energy
- Australia
- Namibia
- ASX Listed
---
