---
description: ''
domains:
- caa:
  - 128 iodef "mailto:9-ait-arin-abuse@faa.gov"
  - 128 issue "digicert.com"
  - 128 issue "amazon.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faa.gov
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.faa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.faa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: external-api.faa.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Federal Aviation Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Aviation Administration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Aviation Administration
provider_slug: federal-aviation-administration
slug: federal-aviation-administration-domain-security
source_filename: federal-aviation-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.faa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.faa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: external-api.faa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: faa.gov\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:9-ait-arin-abuse@faa.gov\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-aviation-administration/refs/heads/main/security/federal-aviation-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Federal Government
---
