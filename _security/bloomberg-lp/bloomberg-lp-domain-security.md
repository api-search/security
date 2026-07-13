---
api_specs:
- filename: openfigi-openapi.yml
  format: yaml
  label: OpenFIGI API
  slug: openfigi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-lp/refs/heads/main/openapi/openfigi-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfigi.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.openfigi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.openfigi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomberg Lp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg L.P., probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg L.P.
provider_slug: bloomberg-lp
slug: bloomberg-lp-domain-security
source_filename: bloomberg-lp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openfigi.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-lp/refs/heads/main/security/bloomberg-lp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Market Data
- News
- Reference Data
- Symbology
- Terminal
---
