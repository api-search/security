---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dtxalliance.org
  spf: true
hosts:
- cert_expires: Nov  3 13:27:38 2026 GMT
  host: dtxalliance.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blue Note Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Note Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Blue Note Therapeutics
provider_slug: blue-note-therapeutics
slug: blue-note-therapeutics-domain-security
source_filename: blue-note-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dtxalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 13:27:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dtxalliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-note-therapeutics/refs/heads/main/security/blue-note-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Digital Therapeutics
- Cancer
- Health
- Biotechnology
---
