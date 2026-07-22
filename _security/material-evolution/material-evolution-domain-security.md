---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: materialevolution.co.uk
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: materialevolution.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Material Evolution Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Material Evolution, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Material Evolution
provider_slug: material-evolution
slug: material-evolution-domain-security
source_filename: material-evolution-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: materialevolution.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: materialevolution.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/material-evolution/refs/heads/main/security/material-evolution-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Cement
- Construction
- Sustainability
- Low Carbon
- Cleantech
- Manufacturing
- Materials
---
