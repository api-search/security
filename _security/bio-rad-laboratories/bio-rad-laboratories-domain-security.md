---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bio-rad.com
  spf: true
hosts:
- cert_expires: Sep 20 13:28:10 2026 GMT
  host: www.bio-rad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bio Rad Laboratories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bio-Rad Laboratories, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bio-Rad Laboratories
provider_slug: bio-rad-laboratories
slug: bio-rad-laboratories-domain-security
source_filename: bio-rad-laboratories-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bio-rad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:28:10 2026 GMT\n  hsts: null\ndomains:\n- domain: bio-rad.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bio-rad-laboratories/refs/heads/main/security/bio-rad-laboratories-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Life Science
- Diagnostics
- Biotechnology
- Research
- Clinical
- Genomics
- Proteomics
- PCR
- Fortune 1000
---
