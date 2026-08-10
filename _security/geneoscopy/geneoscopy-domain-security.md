---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geneoscopy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: colosense.com
  spf: true
hosts:
- cert_expires: Oct 23 13:03:38 2026 GMT
  host: www.geneoscopy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:41:02 2026 GMT
  host: colosense.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geneoscopy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geneoscopy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geneoscopy
provider_slug: geneoscopy
slug: geneoscopy-domain-security
source_filename: geneoscopy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geneoscopy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 13:03:38 2026 GMT\n  hsts: null\n- host: colosense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:41:02 2026 GMT\n  hsts: null\ndomains:\n- domain: geneoscopy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: colosense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geneoscopy/refs/heads/main/security/geneoscopy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Diagnostics
- Molecular Diagnostics
- Colorectal Cancer
- Cancer Screening
- RNA
- Clinical Laboratory
- Life Sciences
- Gastroenterology
---
