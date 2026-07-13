---
api_specs:
- filename: API-Reference
  format: yaml
  label: OpenCorporates API
  slug: open-corporates-api
  spec_type: OpenAPI
  url: https://api.opencorporates.com/documentation/API-Reference
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opencorporates.com
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: opencorporates.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 10:14:02 2026 GMT
  host: api.opencorporates.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Corporates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCorporates, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenCorporates
provider_slug: open-corporates
slug: open-corporates-domain-security
source_filename: open-corporates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencorporates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opencorporates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:14:02 2026 GMT\n  hsts: false\ndomains:\n- domain: opencorporates.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-corporates/refs/heads/main/security/open-corporates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Companies
- Corporate Data
- Business Intelligence
- Compliance
- Due Diligence
- Officers
- Filings
- Corporate Transparency
- Open Data
---
