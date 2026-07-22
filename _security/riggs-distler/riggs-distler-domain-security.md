---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: centuri.com
  spf: true
hosts:
- cert_expires: Sep 28 20:30:17 2026 GMT
  host: centuri.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riggs Distler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riggs Distler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Riggs Distler
provider_slug: riggs-distler
slug: riggs-distler-domain-security
source_filename: riggs-distler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centuri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:30:17 2026 GMT\n  hsts: false\ndomains:\n- domain: centuri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riggs-distler/refs/heads/main/security/riggs-distler-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Electrical
- Utilities
- Energy Infrastructure
---
