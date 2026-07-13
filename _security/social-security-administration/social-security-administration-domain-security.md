---
api_specs:
- filename: ssa-field-office-openapi.yml
  format: yaml
  label: SSA Field Office Address API
  slug: field-office-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/social-security-administration/refs/heads/main/openapi/ssa-field-office-openapi.yml
- filename: ssa-resident-station-openapi.yml
  format: yaml
  label: SSA Resident Station Address API
  slug: resident-station-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/social-security-administration/refs/heads/main/openapi/ssa-resident-station-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ssa.gov
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: www.ssa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services6.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Social Security Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Social Security Administration, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Social Security Administration
provider_slug: social-security-administration
slug: social-security-administration-domain-security
source_filename: social-security-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ssa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\n- host: services6.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ssa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/social-security-administration/refs/heads/main/security/social-security-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Social Security
- Government API
- Open Data
- OASDI
- Disability Benefits
- Retirement Benefits
---
