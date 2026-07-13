---
api_specs:
- filename: varonis-datalert-openapi.yml
  format: yaml
  label: Varonis DatAlert API
  slug: varonis-datalert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/openapi/varonis-datalert-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:soc@varonis.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: varonis.com
  spf: true
hosts:
- cert_expires: Oct  7 11:14:20 2026 GMT
  host: www.varonis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.varonis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Varonis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Varonis, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Varonis
provider_slug: varonis
slug: varonis-domain-security
source_filename: varonis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.varonis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:14:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.varonis.com\n  https: false\ndomains:\n- domain: varonis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:soc@varonis.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/security/varonis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Compliance
- Data Analytics
- Data Governance
- Data Security
- Threat Detection
---
