---
api_specs:
- filename: openapi.json
  format: json
  label: Bloomberg FIGI API
  slug: figi-api
  spec_type: OpenAPI
  url: https://api.openfigi.com/schema/openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfigi.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Bloomberg Proprietary Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg Proprietary Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg Proprietary Technologies
provider_slug: bloomberg-proprietary-technologies
slug: bloomberg-proprietary-technologies-domain-security
source_filename: bloomberg-proprietary-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: www.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openfigi.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-proprietary-technologies/refs/heads/main/security/bloomberg-proprietary-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Proprietary Technology
- BLPAPI
- BQL
- FIGI
- B-PIPE
- Financial Technology
- Bloomberg
---
