---
api_specs:
- filename: lumen-internet-on-demand-api-openapi.yml
  format: yaml
  label: Lumen Internet On-Demand API
  slug: internet-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/openapi/lumen-internet-on-demand-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumen.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.lumen.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developer.lumen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.lumen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumen Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumen Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lumen Technologies
provider_slug: lumen-technologies
slug: lumen-technologies-domain-security
source_filename: lumen-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.lumen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.lumen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lumen.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/security/lumen-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bandwidth
- Edge Cloud
- Fiber
- Infrastructure
- Internet
- Network
- Networking
- Security
- Telecom
---
