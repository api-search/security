---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arpelos.com
  spf: true
hosts:
- cert_expires: Aug 20 09:04:38 2026 GMT
  host: www.arpelos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arpelos Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arpelos Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Arpelos Biosciences
provider_slug: arpelos-biosciences
slug: arpelos-biosciences-domain-security
source_filename: arpelos-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arpelos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:04:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arpelos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arpelos-biosciences/refs/heads/main/security/arpelos-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Drug Discovery
- Protein Engineering
- Computational Biology
---
