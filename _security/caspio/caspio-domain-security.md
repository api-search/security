---
api_specs:
- filename: caspio-openapi.yml
  format: yaml
  label: Caspio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:sysmonitor@caspio.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: true
  domain: caspio.com
  spf: true
hosts:
- cert_expires: Sep 27 15:15:29 2026 GMT
  host: www.caspio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 00:55:31 2026 GMT
  host: howto.caspio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caspio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caspio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Caspio
provider_slug: caspio
slug: caspio-domain-security
source_filename: caspio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caspio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:15:29 2026 GMT\n  hsts: false\n- host: howto.caspio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:55:31 2026 GMT\n  hsts: false\ndomains:\n- domain: caspio.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:sysmonitor@caspio.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/security/caspio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Low Code
- No Code
- Database
- Application Platform
- Cloud Database
- Online Forms
- Workflow Automation
---
