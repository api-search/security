---
api_specs:
- filename: yash12007-openapi-generated.yml
  format: yaml
  label: Yash12007 API
  slug: yash12007-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yash12007/openapi/_ae-authored/yash12007-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yash12007.com
  spf: true
hosts:
- cert_expires: Jan  7 21:11:20 2027 GMT
  host: yash12007.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yash12007 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yash12007, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yash12007
provider_slug: yash12007
slug: yash12007-domain-security
source_filename: yash12007-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yash12007.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 21:11:20 2027 GMT\n  hsts: false\ndomains:\n- domain: yash12007.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/yash12007/security/yash12007-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- Development
- Cloud
- Security
---
