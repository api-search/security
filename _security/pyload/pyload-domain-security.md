---
api_specs:
- filename: pyload-pyload-rest-api-openapi.yml
  format: yaml
  label: pyLoad pyLoad REST API
  slug: pyload-pyload-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyload/openapi/pyload-pyload-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pyload.net
  spf: true
hosts:
- cert_expires: Jan 20 04:07:49 2027 GMT
  host: pyload.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pyload Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pyLoad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: pyLoad
provider_slug: pyload
slug: pyload-domain-security
source_filename: pyload-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pyload.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 04:07:49 2027 GMT\n  hsts: false\ndomains:\n- domain: pyload.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pyload/security/pyload-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Download Manager
- Open Source
- Python
- Automation
- File Transfer
---
