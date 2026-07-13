---
api_specs:
- filename: openapi
  format: yaml
  label: Brandfolder API
  slug: brandfolder-api
  spec_type: OpenAPI
  url: https://developers.smartsheet.com/api/brandfolder/openapi
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@smartsheet.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brandfolder.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@smartsheet.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartsheet.com
  spf: true
hosts:
- cert_expires: Sep 26 03:51:50 2026 GMT
  host: brandfolder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 11:15:38 2026 GMT
  host: developers.smartsheet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandfolder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandfolder, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brandfolder
provider_slug: brandfolder
slug: brandfolder-domain-security
source_filename: brandfolder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandfolder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.smartsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:15:38 2026 GMT\n  hsts: false\ndomains:\n- domain: brandfolder.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@smartsheet.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smartsheet.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@smartsheet.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/security/brandfolder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Brand Management
- Assets
- Media
- Collections
- Smartsheet
---
