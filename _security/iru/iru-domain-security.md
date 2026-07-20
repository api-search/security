---
api_specs:
- filename: how-to-set-up-the-iru-endpoint-api-in-postman.md
  format: yaml
  label: Iru Endpoint Management API
  slug: iru-endpoint-management-api
  spec_type: Postman
  url: https://docs.iru.com/en/endpoint/api/how-to-set-up-the-iru-endpoint-api-in-postman.md
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: iru.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kandji.io
  spf: true
hosts:
- cert_expires: Oct  2 23:57:15 2026 GMT
  host: iru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 20:20:12 2026 GMT
  host: api-docs.iru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 21:02:52 2026 GMT
  host: subdomain.api.kandji.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iru, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Iru
provider_slug: iru
slug: iru-domain-security
source_filename: iru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:57:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.iru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: subdomain.api.kandji.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iru.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kandji.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iru/refs/heads/main/security/iru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Device Management
- Apple MDM
- Endpoint Security
- Identity and Access Management
- Compliance
- Vulnerability Management
- IT Management
- Security
---
