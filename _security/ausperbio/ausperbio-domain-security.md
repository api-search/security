---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ausperbio.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.ausperbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: cms.ausperbio.com
  hsts: false
  https: true
  note: Backend CMS host read from window.SITE_CONFIG['apiURL'] in the ausperbio.com single-page app. Private content-management backend, not a published developer API. No HSTS header and TLS negotiates only 1.2, where the public www host reaches 1.3.
  server: nginx/1.24.0
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ausperbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AusperBio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AusperBio
provider_slug: ausperbio
slug: ausperbio-domain-security
source_filename: ausperbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ausperbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cms.ausperbio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\n  server: nginx/1.24.0\n  note: Backend CMS host read from window.SITE_CONFIG['apiURL'] in the ausperbio.com\n    single-page app. Private content-management backend, not a published developer API.\n    No HSTS header and TLS negotiates only 1.2, where the public www host reaches 1.3.\ndomains:\n- domain: ausperbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ausperbio/refs/heads/main/security/ausperbio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Biopharmaceutical
- Life Sciences
- Therapeutics
- Oligonucleotide
- Antisense Oligonucleotide
- siRNA
- Clinical Trials
- Hepatitis B
- Drug Development
- Health
- China
---
