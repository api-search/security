---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bgov.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: about.bgov.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: api.bgov.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bloomberg Government Bgov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg Government (BGOV), probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg Government (BGOV)
provider_slug: bloomberg-government-bgov
slug: bloomberg-government-bgov-domain-security
source_filename: bloomberg-government-bgov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: about.bgov.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.bgov.com\n  https: false\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bgov.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-government-bgov/refs/heads/main/security/bloomberg-government-bgov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Legislative
- Regulatory
- Government Contracting
- Federal Budget
- Policy Research
- Bloomberg
---
