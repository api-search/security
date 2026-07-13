---
api_specs:
- filename: trelica-rest-api-openapi.yml
  format: yaml
  label: Trelica REST API
  slug: trelica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/openapi/trelica-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:mark.weaver@trelica.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trelica.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.trelica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: trelica.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: app.trelica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trelica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trelica, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trelica
provider_slug: trelica
slug: trelica-domain-security
source_filename: trelica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trelica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trelica.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.trelica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trelica.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:mark.weaver@trelica.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/security/trelica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- IT Management
- License Management
- SaaS Management
- Software Asset Management
---
