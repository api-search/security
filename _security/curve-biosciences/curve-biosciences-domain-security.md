---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curvebio.com
  spf: true
hosts:
- cert_expires: Nov 18 12:35:19 2026 GMT
  host: www.curvebio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curve Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curve Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Curve Biosciences
provider_slug: curve-biosciences
slug: curve-biosciences-domain-security
source_filename: curve-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curvebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 12:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curvebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curve-biosciences/refs/heads/main/security/curve-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Health Tech
- Diagnostics
- Whole-Body Intelligence
---
