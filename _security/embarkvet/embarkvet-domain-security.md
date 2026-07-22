---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: embarkvet.com
  spf: true
hosts:
- cert_expires: Oct  5 20:03:57 2026 GMT
  host: embarkvet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Embarkvet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Embark Veterinary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Embark Veterinary
provider_slug: embarkvet
slug: embarkvet-domain-security
source_filename: embarkvet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: embarkvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:03:57 2026 GMT\n  hsts: false\ndomains:\n- domain: embarkvet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embarkvet/refs/heads/main/security/embarkvet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Canine Genomics
- Dog DNA Test
- Breed Identification
- Genetic Health
- Direct to Consumer
- Pet Tech
- No Public API
---
