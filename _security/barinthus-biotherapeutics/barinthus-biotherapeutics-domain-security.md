---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: barinthusbio.com
  spf: true
hosts:
- cert_expires: Sep 30 09:02:00 2026 GMT
  host: www.barinthusbio.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barinthus Biotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barinthus Biotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Barinthus Biotherapeutics
provider_slug: barinthus-biotherapeutics
slug: barinthus-biotherapeutics-domain-security
source_filename: barinthus-biotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barinthusbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: barinthusbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barinthus-biotherapeutics/refs/heads/main/security/barinthus-biotherapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Biotechnology
- Biopharmaceutical
- Immunotherapy
- Autoimmune
- Oncology
- Clinical Stage
- Life Sciences
---
