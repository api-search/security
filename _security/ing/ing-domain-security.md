---
description: ''
domains:
- caa:
  - 0 issuewild "swisssign.com"
  - 0 issuemail "swisssign.com"
  - 0 issuemail "identrust.com"
  - 0 issuevmc "swisssign.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ing.com
  spf: true
hosts:
- cert_expires: Oct  4 04:59:10 2026 GMT
  host: www.ing.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 12:24:32 2027 GMT
  host: developer.ing.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ING, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ING
provider_slug: ing
slug: ing-domain-security
source_filename: ing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ing.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 12:24:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: ing.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"swisssign.com\"\n  - 0 issuemail \"swisssign.com\"\n  - 0 issuemail \"identrust.com\"\n  - 0 issuevmc \"swisssign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ing/refs/heads/main/security/ing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- European Banking
- Open Banking
- PSD2
---
