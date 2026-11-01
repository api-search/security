---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: singulargenomics.com
  spf: true
hosts:
- cert_expires: Jan  7 11:43:07 2027 GMT
  host: www.singulargenomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Singular Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Singular Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Singular Genomics
provider_slug: singular-genomics
slug: singular-genomics-domain-security
source_filename: singular-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.singulargenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 11:43:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: singulargenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/singular-genomics/security/singular-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Spatial
- Multiomics
- Bioinformatics
---
