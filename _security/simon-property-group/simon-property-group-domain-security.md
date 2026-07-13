---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: simon.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: simonpropertygroup.com
  spf: true
hosts:
- cert_expires: Aug  4 10:40:13 2026 GMT
  host: www.simon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:51:33 2026 GMT
  host: www.simonpropertygroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:40:18 2026 GMT
  host: sellersupport.shopsimon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simon Property Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simon Property Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Simon Property Group
provider_slug: simon-property-group
slug: simon-property-group-domain-security
source_filename: simon-property-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:40:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.simonpropertygroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:51:33 2026 GMT\n  hsts: false\n- host: sellersupport.shopsimon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:40:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simon.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: simonpropertygroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-property-group/refs/heads/main/security/simon-property-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commercial Real Estate
- E-Commerce
- Fortune 500
- Malls
- Outlet Centers
- Real Estate
- REIT
- Retail
---
