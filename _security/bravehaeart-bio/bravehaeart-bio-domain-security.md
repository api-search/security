---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: braveheart.bio
  spf: true
hosts:
- cert_expires: Nov 24 23:29:57 2026 GMT
  host: www.braveheart.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bravehaeart Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bravehaeart Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bravehaeart Bio
provider_slug: bravehaeart-bio
slug: bravehaeart-bio-domain-security
source_filename: bravehaeart-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braveheart.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:29:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: braveheart.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bravehaeart-bio/refs/heads/main/security/bravehaeart-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Biotechnology
- Cardiology
- Rare Disease
- Therapeutics
- Gene Editing
- Company
---
