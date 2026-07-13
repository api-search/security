---
api_specs:
- filename: medidata-rave-openapi.yml
  format: yaml
  label: Medidata Rave EDC API
  slug: medidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-rave-openapi.yml
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
hosts:
- cert_expires: Sep 20 03:33:06 2026 GMT
  host: www.medidata.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- host: developer.medidata.com
  https: false
kind: domain-security
layout: security
method: probed
name: Medidata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for medidata, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: medidata
provider_slug: medidata
slug: medidata-domain-security
source_filename: medidata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medidata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 03:33:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.medidata.com\n  https: false\ndomains:\n- domain: medidata.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/security/medidata-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags: []
---
