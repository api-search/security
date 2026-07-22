---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arrakistx.com
  spf: true
hosts:
- cert_expires: Oct  8 19:15:19 2026 GMT
  host: www.arrakistx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arrakis Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arrakis Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arrakis Therapeutics
provider_slug: arrakis-therapeutics
slug: arrakis-therapeutics-domain-security
source_filename: arrakis-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arrakistx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:15:19 2026 GMT\n  hsts: false\ndomains:\n- domain: arrakistx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arrakis-therapeutics/refs/heads/main/security/arrakis-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceutical
- RNA
- Drug Discovery
- Genetic Medicine
- Small Molecules
- Life Sciences
---
