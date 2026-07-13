---
api_specs:
- filename: icims-openapi.yml
  format: yaml
  label: iCIMS Workflows API
  slug: icims-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icims/refs/heads/main/openapi/icims-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domains@icims.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icims.com
  spf: true
hosts:
- cert_expires: Aug  9 19:28:12 2026 GMT
  host: developer-community.icims.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 00:15:12 2026 GMT
  host: www.icims.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 23:59:59 2026 GMT
  host: api.icims.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Icims Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iCIMS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iCIMS
provider_slug: icims
slug: icims-domain-security
source_filename: icims-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-community.icims.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 19:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.icims.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:15:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: api.icims.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: icims.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domains@icims.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icims/refs/heads/main/security/icims-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Applicant Tracking
- HR
- Recruiting
- Talent Acquisition
---
