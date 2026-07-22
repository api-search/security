---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mammoth.bio
  spf: false
hosts:
- cert_expires: Oct 15 15:05:48 2026 GMT
  host: mammoth.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mammoth Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mammoth Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mammoth Biosciences
provider_slug: mammoth-biosciences
slug: mammoth-biosciences-domain-security
source_filename: mammoth-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mammoth.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:05:48 2026 GMT\n  hsts: false\ndomains:\n- domain: mammoth.bio\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mammoth-biosciences/refs/heads/main/security/mammoth-biosciences-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- CRISPR
- Gene Editing
- Genetic Medicine
- Diagnostics
- Therapeutics
---
