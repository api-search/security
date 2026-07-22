---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: transposonrx.com
  spf: true
hosts:
- cert_expires: Oct 14 15:32:31 2026 GMT
  host: transposonrx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transposon Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transposon Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transposon Therapeutics
provider_slug: transposon-therapeutics
slug: transposon-therapeutics-domain-security
source_filename: transposon-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transposonrx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 15:32:31 2026 GMT\n  hsts: false\ndomains:\n- domain: transposonrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transposon-therapeutics/refs/heads/main/security/transposon-therapeutics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Neurodegeneration
- Clinical Stage
- Drug Development
- Life Sciences
- Neuroscience
---
