---
api_specs:
- filename: isbusinessemail-check-api-openapi.yml
  format: yaml
  label: isBusinessEmail Check API
  slug: isbusinessemail-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-check-api-openapi.yml
- filename: isbusinessemail-feedback-api-openapi.yml
  format: yaml
  label: isBusinessEmail Feedback API
  slug: isbusinessemail-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-feedback-api-openapi.yml
- filename: isbusinessemail-health-api-openapi.yml
  format: yaml
  label: isBusinessEmail Health API
  slug: isbusinessemail-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-health-api-openapi.yml
- filename: isbusinessemail-usage-api-openapi.yml
  format: yaml
  label: isBusinessEmail Usage API
  slug: isbusinessemail-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: isbusinessemail.com
  spf: true
hosts:
- cert_expires: Jan  2 17:17:58 2027 GMT
  host: isbusinessemail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Isbusinessemail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for isBusinessEmail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: isBusinessEmail
provider_slug: isbusinessemail
slug: isbusinessemail-domain-security
source_filename: isbusinessemail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isbusinessemail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 17:17:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: isbusinessemail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/security/isbusinessemail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EmailVerification
- BusinessTools
- EUHosted
---
