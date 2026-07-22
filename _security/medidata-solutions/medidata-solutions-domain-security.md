---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "globalsign.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medidata.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "globalsign.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mdsol.com
  spf: true
hosts:
- cert_expires: Sep 20 03:33:06 2026 GMT
  host: www.medidata.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: innovate.mdsol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medidata Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medidata Solutions, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medidata Solutions
provider_slug: medidata-solutions
slug: medidata-solutions-domain-security
source_filename: medidata-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medidata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 03:33:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: innovate.mdsol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: medidata.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mdsol.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata-solutions/refs/heads/main/security/medidata-solutions-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Healthcare
- Clinical Trials
- Life Sciences
- Electronic Data Capture
- EDC
- Pharma
- CDISC ODM
- Clinical Data Management
- Dassault Systemes
---
