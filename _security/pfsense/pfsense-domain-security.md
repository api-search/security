---
api_specs:
- filename: pfsense-openapi.yml
  format: yaml
  label: pfSense REST API (pfSense-pkg-RESTAPI)
  slug: rest-api-package
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pfsense/refs/heads/main/openapi/pfsense-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pfsense.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pfrest.org
  spf: true
hosts:
- cert_expires: Sep 30 12:08:08 2026 GMT
  host: www.pfsense.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 20:57:49 2026 GMT
  host: pfrest.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: pfsense.local
  https: false
kind: domain-security
layout: security
method: probed
name: Pfsense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pfSense, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: pfSense
provider_slug: pfsense
slug: pfsense-domain-security
source_filename: pfsense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pfsense.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pfrest.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: pfsense.local\n  https: false\ndomains:\n- domain: pfsense.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pfrest.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pfsense/refs/heads/main/security/pfsense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Firewall
- Network Security
- Router
- VPN
- Open Source
- FreeBSD
- Netgate
---
