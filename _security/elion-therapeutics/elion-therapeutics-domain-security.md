---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eliontx.com
  spf: true
hosts:
- cert_expires: Oct 22 06:31:38 2026 GMT
  host: eliontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elion Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elion Therapeutics
provider_slug: elion-therapeutics
slug: elion-therapeutics-domain-security
source_filename: elion-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eliontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 06:31:38 2026 GMT\n  hsts: false\ndomains:\n- domain: eliontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elion-therapeutics/refs/heads/main/security/elion-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Therapeutics
- Life Sciences
- Anti-Infectives
- Drug Development
- Clinical Stage
- Healthcare
---
