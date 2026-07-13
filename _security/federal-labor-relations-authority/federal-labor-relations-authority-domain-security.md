---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: flra.gov
  spf: true
hosts:
- cert_expires: Sep  5 12:41:27 2026 GMT
  host: www.flra.gov
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Federal Labor Relations Authority Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Labor Relations Authority, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Labor Relations Authority
provider_slug: federal-labor-relations-authority
slug: federal-labor-relations-authority-domain-security
source_filename: federal-labor-relations-authority-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flra.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 12:41:27 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: flra.gov\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-labor-relations-authority/refs/heads/main/security/federal-labor-relations-authority-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Labor
---
