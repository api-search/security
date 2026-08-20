---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claimgenius.com
  spf: true
hosts:
- cert_expires: Oct 25 04:53:00 2026 GMT
  host: claimgenius.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claim Genius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claim Genius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claim Genius
provider_slug: claim-genius
slug: claim-genius-domain-security
source_filename: claim-genius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claimgenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 04:53:00 2026 GMT\n  hsts: false\ndomains:\n- domain: claimgenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claim-genius/refs/heads/main/security/claim-genius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Insurance Claims
- Insurance Underwriting
- Artificial Intelligence
- Computer-Vision
- Vehicle Inspection
- Automotive
- Claims Automation
- Damage Assessment
- Insurtech
---
