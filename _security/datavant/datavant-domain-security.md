---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datavant.com
  spf: true
hosts:
- cert_expires: Sep 16 02:30:59 2026 GMT
  host: www.datavant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datavant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datavant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Datavant
provider_slug: datavant
slug: datavant-domain-security
source_filename: datavant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datavant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:30:59 2026 GMT\n  hsts: false\ndomains:\n- domain: datavant.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/security/datavant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
---
