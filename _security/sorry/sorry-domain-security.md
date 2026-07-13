---
api_specs:
- filename: sorry-status-page-openapi.yml
  format: yaml
  label: Sorry Status Page API
  slug: sorry-status-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorry/refs/heads/main/openapi/sorry-status-page-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:webservices+caa@sorryapp.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sorryapp.com
  spf: true
hosts:
- cert_expires: Aug 11 08:23:57 2026 GMT
  host: www.sorryapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 11:27:02 2026 GMT
  host: docs.sorryapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 17:53:49 2026 GMT
  host: api.sorryapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sorry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorry, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sorry
provider_slug: sorry
slug: sorry-domain-security
source_filename: sorry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sorryapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 08:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sorryapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sorryapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:53:49 2026 GMT\n  hsts: null\ndomains:\n- domain: sorryapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:webservices+caa@sorryapp.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorry/refs/heads/main/security/sorry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Status Pages
- Incident Management
- Developer Tools
- Monitoring
- Notifications
---
