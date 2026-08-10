---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trex.bio
  spf: true
hosts:
- cert_expires: Sep 25 08:29:21 2026 GMT
  host: trex.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trexbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRexBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TRexBio
provider_slug: trexbio
slug: trexbio-domain-security
source_filename: trexbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trex.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:29:21 2026 GMT\n  hsts: false\ndomains:\n- domain: trex.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trexbio/refs/heads/main/security/trexbio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Immunology
- Drug Discovery
- Regulatory T Cells
- Clinical Stage
- Computational Biology
- Therapeutics
- South San Francisco
---
