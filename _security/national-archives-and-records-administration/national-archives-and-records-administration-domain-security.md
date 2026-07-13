---
api_specs:
- filename: national-archives-and-records-administration-openapi.json
  format: json
  label: National Archives Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-archives-and-records-administration/main/openapi/national-archives-and-records-administration-openapi.json
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: archives.gov
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.archives.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: catalog.archives.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Archives And Records Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Archives and Records Administration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Archives and Records Administration
provider_slug: national-archives-and-records-administration
slug: national-archives-and-records-administration-domain-security
source_filename: national-archives-and-records-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archives.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: catalog.archives.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: archives.gov\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-archives-and-records-administration/refs/heads/main/security/national-archives-and-records-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Archives
- Federal Government
- Records
- Catalog
---
