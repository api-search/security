---
api_specs:
- filename: affise-postman-api-collection
  format: yaml
  label: Affise Performance API
  slug: affise-performance-api
  spec_type: Postman
  url: https://github.com/affise/affise-postman-api-collection
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affise.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intercom.help
  spf: false
hosts:
- cert_expires: Nov 26 15:42:52 2026 GMT
  host: affise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 15:42:52 2026 GMT
  host: api.affise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: intercom.help
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Affise
provider_slug: affise
slug: affise-domain-security
source_filename: affise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 15:42:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.affise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 15:42:52 2026 GMT\n  hsts: false\n- host: intercom.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: affise.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: intercom.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affise/refs/heads/main/security/affise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Performance Marketing
- Conversions
- Publishers
- Analytics
- Attribution
---
