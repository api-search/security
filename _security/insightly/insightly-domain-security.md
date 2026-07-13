---
api_specs:
- filename: insightly-openapi.yml
  format: yaml
  label: Insightly REST API v3.1
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/openapi/insightly-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: insightly.com
  spf: true
hosts:
- cert_expires: Sep 23 14:53:23 2026 GMT
  host: www.insightly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.insightly.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Insightly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insightly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Insightly
provider_slug: insightly
slug: insightly-domain-security
source_filename: insightly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insightly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:53:23 2026 GMT\n  hsts: false\n- host: api.insightly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: insightly.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insightly/refs/heads/main/security/insightly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Project Management
- Lead Management
- Opportunities
- Contacts
- SMB
---
