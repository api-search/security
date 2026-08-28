---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: paqtx.com
  spf: true
hosts:
- cert_expires: Oct 20 05:23:59 2026 GMT
  host: www.paqtx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paq Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PAQ Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PAQ Therapeutics
provider_slug: paq-therapeutics
slug: paq-therapeutics-domain-security
source_filename: paq-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paqtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:23:59 2026 GMT\n  hsts: false\ndomains:\n- domain: paqtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paq-therapeutics/refs/heads/main/security/paq-therapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Therapeutics
- Drug Discovery
- Targeted Protein Degradation
- Life Sciences
- Clinical Stage
- Massachusetts
---
