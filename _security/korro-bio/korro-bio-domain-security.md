---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: korrobio.com
  spf: true
hosts:
- cert_expires: Dec  3 11:04:34 2026 GMT
  host: korrobio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Korro Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korro Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Korro Bio
provider_slug: korro-bio
slug: korro-bio-domain-security
source_filename: korro-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: korrobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 11:04:34 2026 GMT\n  hsts: false\ndomains:\n- domain: korrobio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korro-bio/refs/heads/main/security/korro-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- RNA Editing
- Genetic Medicine
- Drug Discovery
- Life Sciences
- Clinical Trials
- Rare Disease
- Research
---
