---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bambusatx.com
  spf: true
hosts:
- cert_expires: Sep 16 14:17:48 2026 GMT
  host: bambusatx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bambusa Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bambusa Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bambusa Therapeutics
provider_slug: bambusa-therapeutics
slug: bambusa-therapeutics-domain-security
source_filename: bambusa-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bambusatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:17:48 2026 GMT\n  hsts: false\ndomains:\n- domain: bambusatx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bambusa-therapeutics/refs/heads/main/security/bambusa-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Immunology
- Clinical Trials
- Drug Development
- Antibodies
---
