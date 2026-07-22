---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: origin.bio
  spf: true
hosts:
- cert_expires: Sep 11 12:23:50 2026 GMT
  host: origin.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Origin Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Origin Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Origin Bio
provider_slug: origin-bio
slug: origin-bio-domain-security
source_filename: origin-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: origin.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:23:50 2026 GMT\n  hsts: false\ndomains:\n- domain: origin.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin-bio/refs/heads/main/security/origin-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Cancer Research
- Spatial Genomics
- Transcriptomics
- Artificial Intelligence
- Life Sciences
- Y Combinator
---
