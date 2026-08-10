---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: generalfusion.com
  spf: true
hosts:
- cert_expires: Sep 29 04:44:18 2026 GMT
  host: generalfusion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Fusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Fusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: General Fusion
provider_slug: general-fusion
slug: general-fusion-domain-security
source_filename: general-fusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the General Fusion web host\nnote: Third-party hosts referenced from apis.yml (the Hiive secondary-market listing)\n  were probed but are excluded here; this artifact records only hosts General Fusion\n  operates.\nhosts:\n- host: generalfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:44:18 2026 GMT\n  hsts: null\ndomains:\n- domain: generalfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-fusion/refs/heads/main/security/general-fusion-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Fusion Energy
- Clean Energy
- Nuclear Fusion
- Deep Tech
- Research
- Canada
---
