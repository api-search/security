---
api_specs:
- filename: technology-standards-openapi.yml
  format: yaml
  label: IETF Internet Standards
  slug: ietf-standards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/technology-standards/refs/heads/main/openapi/technology-standards-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sysreq@w3.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w3.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: www.ietf.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: www.w3.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 09:19:38 2026 GMT
  host: standards.ieee.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Technology Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technology Standards, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Technology Standards
provider_slug: technology-standards
slug: technology-standards-domain-security
source_filename: technology-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: false\n- host: www.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: standards.ieee.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:19:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: w3.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sysreq@w3.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/technology-standards/refs/heads/main/security/technology-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IEEE
- IETF
- ISO
- Protocols
- Standards
- Technology Standards
- W3C
---
