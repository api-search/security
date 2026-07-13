---
api_specs:
- filename: saviynt-eic-api_openapi3.yaml
  format: yaml
  label: Saviynt Enterprise Identity Cloud API
  slug: saviynt-enterprise-identity-cloud-api
  spec_type: OpenAPI
  url: https://github.com/vivek9237/saviynt-api-reference/blob/main/docs/saviynt-eic-api_openapi3.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: saviynt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saviyntcloud.com
  spf: true
hosts:
- cert_expires: Sep  5 20:24:58 2026 GMT
  host: saviynt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developers.saviynt.com
  https: false
- host: example.saviyntcloud.com
  https: false
kind: domain-security
layout: security
method: probed
name: Saviynt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saviynt, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Saviynt
provider_slug: saviynt
slug: saviynt-domain-security
source_filename: saviynt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saviynt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.saviynt.com\n  https: false\n- host: example.saviyntcloud.com\n  https: false\ndomains:\n- domain: saviynt.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: saviyntcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saviynt/refs/heads/main/security/saviynt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Governance
- Identity Administration
- Access Management
- Privileged Access Management
- Segregation of Duties
- IGA
- Security
---
