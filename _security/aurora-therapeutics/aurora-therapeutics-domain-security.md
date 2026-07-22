---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auroratherapeutics.com
  spf: true
hosts:
- cert_expires: Sep 25 22:13:52 2026 GMT
  host: auroratherapeutics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurora Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aurora Therapeutics
provider_slug: aurora-therapeutics
slug: aurora-therapeutics-domain-security
source_filename: aurora-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auroratherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: auroratherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-therapeutics/refs/heads/main/security/aurora-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Gene Editing
- CRISPR
- Rare Disease
- Personalized Medicine
- Therapeutics
---
