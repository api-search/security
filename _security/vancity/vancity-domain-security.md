---
description: ''
domains:
- caa:
  - 0 iodef "mailto:webmaster@vancity.com"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vancity.com
  spf: true
hosts:
- cert_expires: Feb 22 00:09:02 2027 GMT
  host: www.vancity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vancity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vancity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vancity
provider_slug: vancity
slug: vancity-domain-security
source_filename: vancity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vancity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 00:09:02 2027 GMT\n  hsts: null\ndomains:\n- domain: vancity.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:webmaster@vancity.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vancity/refs/heads/main/security/vancity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Co-operative
- Interac
- Payments
- Data Aggregation
---
