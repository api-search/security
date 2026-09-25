---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 32biosciences.com
  spf: true
hosts:
- cert_expires: Nov  8 20:56:47 2026 GMT
  host: 32biosciences.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 32 Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 32 Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 32 Biosciences
provider_slug: 32-biosciences
slug: 32-biosciences-domain-security
source_filename: 32-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 32biosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 20:56:47 2026 GMT\n  hsts: false\ndomains:\n- domain: 32biosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/32-biosciences/refs/heads/main/security/32-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Gastroenterology
- Microbiome
- Diagnostics
- Therapeutics
- Drug Discovery
- Pharmaceuticals
- Metabolomics
- Healthcare
---
