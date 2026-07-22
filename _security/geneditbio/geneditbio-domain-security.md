---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geneditbio.com
  spf: true
hosts:
- cert_expires: Sep  9 17:44:03 2026 GMT
  host: geneditbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geneditbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreezeBio (formerly GenEdit), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BreezeBio (formerly GenEdit)
provider_slug: geneditbio
slug: geneditbio-domain-security
source_filename: geneditbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geneditbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:44:03 2026 GMT\n  hsts: false\ndomains:\n- domain: geneditbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geneditbio/refs/heads/main/security/geneditbio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Genetic Medicine
- Gene Editing
- Drug Delivery
- Nanoparticles
- CRISPR
- Therapeutics
- Life Sciences
- Healthcare
---
