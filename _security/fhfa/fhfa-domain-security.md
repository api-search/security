---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fhfa.gov
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.fhfa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fhfa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Housing Finance Agency (FHFA), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Housing Finance Agency (FHFA)
provider_slug: fhfa
slug: fhfa-domain-security
source_filename: fhfa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fhfa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fhfa.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fhfa/refs/heads/main/security/fhfa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Housing Finance
- House Price Index
- Mortgage
- Government
- GSE
- Fannie Mae
- Freddie Mac
- Federal
---
