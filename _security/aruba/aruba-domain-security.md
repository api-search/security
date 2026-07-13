---
api_specs:
- filename: aruba-central-api.yml
  format: yaml
  label: Aruba Central API
  slug: aruba-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-central-api.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arubanetworks.com
  spf: true
hosts:
- cert_expires: Sep 13 04:50:11 2026 GMT
  host: developer.arubanetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: apigw-prod2.central.arubanetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.arubanetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aruba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aruba, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aruba
provider_slug: aruba
slug: aruba-domain-security
source_filename: aruba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.arubanetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:50:11 2026 GMT\n  hsts: false\n- host: apigw-prod2.central.arubanetworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\n- host: www.arubanetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arubanetworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/security/aruba-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
---
