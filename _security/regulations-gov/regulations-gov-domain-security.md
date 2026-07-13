---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Regulations.gov API
  slug: regulations-gov-api
  spec_type: OpenAPI
  url: https://api.regulations.gov/v4/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: regulations.gov
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issuewild "comodoca.com"
  - 0 iodef "mailto:hostmaster@gsa.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gsa.gov
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.regulations.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 10:21:32 2026 GMT
  host: open.gsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 17:21:20 2026 GMT
  host: api.regulations.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regulations Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regulations.gov, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Regulations.gov
provider_slug: regulations-gov
slug: regulations-gov-domain-security
source_filename: regulations-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regulations.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\n- host: open.gsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.regulations.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 17:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: regulations.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gsa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 iodef \"mailto:hostmaster@gsa.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/security/regulations-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Federal Rulemaking
- Public Comments
- Regulatory
- Dockets
- GSA
- Open Data
---
