---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vizgen.com
  spf: true
hosts:
- cert_expires: Oct 15 03:29:34 2026 GMT
  host: vizgen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vizgen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vizgen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vizgen
provider_slug: vizgen
slug: vizgen-domain-security
source_filename: vizgen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vizgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:29:34 2026 GMT\n  hsts: false\ndomains:\n- domain: vizgen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vizgen/refs/heads/main/security/vizgen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spatial Biology
- Spatial Transcriptomics
- Genomics
- Life Sciences
- Bioinformatics
- Single Cell Analysis
- Scientific Instruments
- Open-Source
- Command Line Tools
---
