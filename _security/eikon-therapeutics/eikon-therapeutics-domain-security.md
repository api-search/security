---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eikontx.com
  spf: true
hosts:
- cert_expires: Sep  7 02:31:46 2026 GMT
  host: eikontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eikon Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eikon Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eikon Therapeutics
provider_slug: eikon-therapeutics
slug: eikon-therapeutics-domain-security
source_filename: eikon-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eikontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:31:46 2026 GMT\n  hsts: false\ndomains:\n- domain: eikontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eikon-therapeutics/refs/heads/main/security/eikon-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Biopharmaceutical
- Drug Discovery
- Live-Cell Imaging
- Super-Resolution Microscopy
- Oncology
- Life Sciences
---
