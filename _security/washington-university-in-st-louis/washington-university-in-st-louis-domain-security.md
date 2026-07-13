---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wustl.edu
  spf: true
hosts:
- cert_expires: Sep  4 17:25:39 2026 GMT
  host: wustl.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:03:12 2026 GMT
  host: data.wustl.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 12:10:36 2026 GMT
  host: digitalcommonsdata.wustl.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Washington University In St Louis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Washington University in St. Louis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Washington University in St. Louis
provider_slug: washington-university-in-st-louis
slug: washington-university-in-st-louis-domain-security
source_filename: washington-university-in-st-louis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wustl.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:25:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: data.wustl.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:03:12 2026 GMT\n  hsts: false\n- host: digitalcommonsdata.wustl.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wustl.edu\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/washington-university-in-st-louis/refs/heads/main/security/washington-university-in-st-louis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United States
- MuleSoft
- OAI-PMH
---
