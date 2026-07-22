---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elegenbio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: elegen.com
  spf: true
hosts:
- cert_expires: Sep 19 19:09:49 2026 GMT
  host: elegenbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: ecommerce.elegen.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elegen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elegen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elegen
provider_slug: elegen
slug: elegen-domain-security
source_filename: elegen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elegenbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:09:49 2026 GMT\n  hsts: false\n- host: ecommerce.elegen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: elegenbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: elegen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elegen/refs/heads/main/security/elegen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Synthetic Biology
- DNA Synthesis
- Biotechnology
- Genomics
- Gene Synthesis
- Life Sciences
- mRNA
- Cell and Gene Therapy
- Synthetic DNA
---
