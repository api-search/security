---
api_specs:
- filename: infoblox-wapi-openapi.yml
  format: yaml
  label: Infoblox WAPI (Web API)
  slug: infoblox-wapi-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoblox/refs/heads/main/openapi/infoblox-wapi-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Infoblox BloxOne API
  slug: infoblox-bloxone-api
  spec_type: OpenAPI
  url: https://csp.infoblox.com/apidoc/
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issuevmc "digicert.com"
  - 0 issuemail "digicert.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infoblox.com
  spf: true
hosts:
- cert_expires: Aug 13 06:17:47 2026 GMT
  host: www.infoblox.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: csp.infoblox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 21:29:52 2026 GMT
  host: docs.infoblox.com
  hsts: true
  hsts_max_age: 34560000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infoblox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infoblox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Infoblox
provider_slug: infoblox
slug: infoblox-domain-security
source_filename: infoblox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infoblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 06:17:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: csp.infoblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.infoblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 34560000\ndomains:\n- domain: infoblox.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuevmc \"digicert.com\"\n  - 0 issuemail \"digicert.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoblox/refs/heads/main/security/infoblox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud
- DDI
- DHCP
- DNS
- IPAM
- Network Management
- Security
- Threat Intelligence
---
