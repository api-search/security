---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:developer+dns@simpplr.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: simpplr.com
  spf: true
hosts:
- cert_expires: Sep 10 21:48:39 2026 GMT
  host: simpplr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:12:40 2026 GMT
  host: developer.simpplr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: api.ec.simpplr.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Simpplr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simpplr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Simpplr
provider_slug: simpplr
slug: simpplr-domain-security
source_filename: simpplr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpplr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:48:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.simpplr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ec.simpplr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: simpplr.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:developer+dns@simpplr.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/security/simpplr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Employee Experience
- Intranet
- Employee Communications
- Digital Workplace
- Internal Communications
- HR
- Collaboration
- Enterprise Software
- Salesforce
---
