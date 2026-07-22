---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hongene.com
  spf: true
hosts:
- cert_expires: Oct 14 10:47:47 2026 GMT
  host: www.hongene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hongene Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hongene Biotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hongene Biotech
provider_slug: hongene-biotech
slug: hongene-biotech-domain-security
source_filename: hongene-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hongene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:47:47 2026 GMT\n  hsts: false\ndomains:\n- domain: hongene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hongene-biotech/refs/heads/main/security/hongene-biotech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- CDMO
- Nucleic Acids
- Oligonucleotide
- mRNA
- Pharmaceutical Manufacturing
- RNA Therapeutics
---
