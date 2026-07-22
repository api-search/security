---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humanegenomics.com
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: humanegenomics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humane Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humane Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Humane Genomics
provider_slug: humane-genomics
slug: humane-genomics-domain-security
source_filename: humane-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanegenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: humanegenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humane-genomics/refs/heads/main/security/humane-genomics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Genomics
- Oncology
- Therapeutics
- Cancer
- Synthetic Biology
---
