---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloriontx.com
  spf: true
hosts:
- cert_expires: Oct 17 14:34:20 2026 GMT
  host: alloriontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allorion Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allorion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allorion Therapeutics
provider_slug: allorion-therapeutics
slug: allorion-therapeutics-domain-security
source_filename: allorion-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloriontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:34:20 2026 GMT\n  hsts: false\ndomains:\n- domain: alloriontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allorion-therapeutics/refs/heads/main/security/allorion-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Oncology
- Autoimmune
- Life Sciences
- Clinical Stage
---
