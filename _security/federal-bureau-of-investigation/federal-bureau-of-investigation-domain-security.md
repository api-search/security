---
api_specs:
- filename: most-wanted-api-openapi.yml
  format: yaml
  label: FBI Most Wanted
  slug: most-wanted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-bureau-of-investigation/refs/heads/main/openapi/most-wanted-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fbi.gov
  spf: true
hosts:
- cert_expires: Oct  8 01:34:31 2026 GMT
  host: www.fbi.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 12:46:39 2026 GMT
  host: api.fbi.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: crime-data-explorer.fbi.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Federal Bureau Of Investigation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Bureau of Investigation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Bureau of Investigation
provider_slug: federal-bureau-of-investigation
slug: federal-bureau-of-investigation-domain-security
source_filename: federal-bureau-of-investigation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fbi.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fbi.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:46:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: crime-data-explorer.fbi.gov\n  https: false\ndomains:\n- domain: fbi.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-bureau-of-investigation/refs/heads/main/security/federal-bureau-of-investigation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FBI
- Federal Government
---
