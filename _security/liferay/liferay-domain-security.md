---
api_specs:
- filename: liferay-openapi.yml
  format: yaml
  label: Liferay Roles API
  slug: liferay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/openapi/liferay-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: liferay.com
  spf: true
hosts:
- cert_expires: Oct  7 18:48:19 2026 GMT
  host: learn.liferay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liferay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liferay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Liferay
provider_slug: liferay
slug: liferay-domain-security
source_filename: liferay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.liferay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liferay.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/security/liferay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Source
- Digital Experience
- DXP
- Roles
- Users
- Permissions
- Headless
---
