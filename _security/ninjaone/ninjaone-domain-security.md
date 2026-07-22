---
api_specs:
- filename: ninjaone-openapi-original.yml
  format: yaml
  label: NinjaOne Public API 2.0
  slug: ninjaone-public-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/openapi/ninjaone-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ninjaone.com
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ninjarmm.com
  spf: true
hosts:
- cert_expires: Sep 15 00:16:39 2026 GMT
  host: www.ninjaone.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: app.ninjarmm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ninjaone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NinjaOne, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NinjaOne
provider_slug: ninjaone
slug: ninjaone-domain-security
source_filename: ninjaone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ninjaone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.ninjarmm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ninjaone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ninjarmm.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/security/ninjaone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- IT Management
- RMM
- Endpoint Management
- MSP
- IT Operations
- Monitoring
- Automation
- Ticketing
---
