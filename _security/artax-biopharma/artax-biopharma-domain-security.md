---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artaxbiopharma.com
  spf: true
hosts:
- cert_expires: Oct 26 23:07:21 2026 GMT
  host: artaxbiopharma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artax Biopharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artax Biopharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Artax Biopharma
provider_slug: artax-biopharma
slug: artax-biopharma-domain-security
source_filename: artax-biopharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artaxbiopharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:07:21 2026 GMT\n  hsts: null\ndomains:\n- domain: artaxbiopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artax-biopharma/refs/heads/main/security/artax-biopharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Clinical-stage
- Autoimmune
- Immunomodulation
- Nck-modulators
---
