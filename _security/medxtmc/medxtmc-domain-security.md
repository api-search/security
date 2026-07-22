---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medxtmc.net
  spf: false
hosts:
- cert_expires: Oct  2 01:59:59 2026 GMT
  host: www.medxtmc.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Medxtmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for medxtmc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: medxtmc
provider_slug: medxtmc
slug: medxtmc-domain-security
source_filename: medxtmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medxtmc.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 01:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: medxtmc.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medxtmc/refs/heads/main/security/medxtmc-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Precision Medicine
- Companion Diagnostics
- Molecular Diagnostics
- Biomarkers
- Clinical Testing
- Healthcare
- Life Sciences
---
