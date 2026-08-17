---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geneostx.com
  spf: true
hosts:
- cert_expires: Oct 15 17:52:46 2026 GMT
  host: www.geneostx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geneos Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geneos Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Geneos Therapeutics
provider_slug: geneos-therapeutics
slug: geneos-therapeutics-domain-security
source_filename: geneos-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geneostx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:52:46 2026 GMT\n  hsts: false\ndomains:\n- domain: geneostx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geneos-therapeutics/refs/heads/main/security/geneos-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Immunotherapy
- Oncology
- Precision Medicine
- Clinical Stage
- Life Sciences
---
