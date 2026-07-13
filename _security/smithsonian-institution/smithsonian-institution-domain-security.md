---
api_specs:
- filename: smithsonian-open-access-openapi.yml
  format: yaml
  label: Smithsonian Open Access API
  slug: open-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/openapi/smithsonian-open-access-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: si.edu
  spf: true
hosts:
- cert_expires: Aug 16 09:59:07 2026 GMT
  host: www.si.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: edan.si.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smithsonian Institution Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smithsonian Institution, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Smithsonian Institution
provider_slug: smithsonian-institution
slug: smithsonian-institution-domain-security
source_filename: smithsonian-institution-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.si.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:59:07 2026 GMT\n  hsts: false\n- host: edan.si.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: si.edu\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/security/smithsonian-institution-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Collections
- Cultural Heritage
- Museums
- Open Data
- Art
- Natural History
- Research
---
