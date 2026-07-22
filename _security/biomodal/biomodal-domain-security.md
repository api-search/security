---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biomodal.com
  spf: true
hosts:
- cert_expires: Sep 25 14:42:02 2026 GMT
  host: biomodal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biomodal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biomodal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biomodal
provider_slug: biomodal
slug: biomodal-domain-security
source_filename: biomodal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biomodal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:42:02 2026 GMT\n  hsts: false\ndomains:\n- domain: biomodal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biomodal/refs/heads/main/security/biomodal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Genomics
- Epigenetics
- Multiomics
- DNA Sequencing
- Bioinformatics
- Precision Medicine
---
