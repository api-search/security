---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bostongene.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: site.com
  spf: true
hosts:
- cert_expires: Oct 10 21:11:59 2026 GMT
  host: bostongene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: bostongene.my.site.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bostongene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BostonGene, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BostonGene
provider_slug: bostongene
slug: bostongene-domain-security
source_filename: bostongene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bostongene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:11:59 2026 GMT\n  hsts: false\n- host: bostongene.my.site.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bostongene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: site.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bostongene/refs/heads/main/security/bostongene-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health Care
- Oncology
- Precision Medicine
- Genomics
- Bioinformatics
- Artificial Intelligence
- Diagnostics
- Life Sciences
- Clinical Laboratory
---
