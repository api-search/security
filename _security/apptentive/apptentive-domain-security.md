---
api_specs:
- filename: apptentive-openapi-original.yml
  format: yaml
  label: Apptentive Data API
  slug: apptentive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/openapi/apptentive-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apptentive.com
  spf: true
hosts:
- cert_expires: Oct  5 00:33:15 2026 GMT
  host: apptentive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 14:05:52 2026 GMT
  host: data.apptentive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apptentive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apptentive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apptentive
provider_slug: apptentive
slug: apptentive-domain-security
source_filename: apptentive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apptentive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:33:15 2026 GMT\n  hsts: null\n- host: data.apptentive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:05:52 2026 GMT\n  hsts: null\ndomains:\n- domain: apptentive.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/security/apptentive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Mobile
- Customer Feedback
- Surveys
- Analytics
- Customer Engagement
- Voice of Customer
---
