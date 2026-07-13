---
api_specs:
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Bonuses API
  slug: bonusly-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Users API
  slug: bonusly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Rewards API
  slug: bonusly-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Redemptions API
  slug: bonusly-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Analytics API
  slug: bonusly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Company API
  slug: bonusly-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bonusly.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bonus.ly
  spf: true
hosts:
- cert_expires: Sep 30 09:38:35 2026 GMT
  host: bonusly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:54:27 2026 GMT
  host: docs.bonus.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 12:32:11 2026 GMT
  host: bonus.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bonusly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonusly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bonusly
provider_slug: bonusly
slug: bonusly-domain-security
source_filename: bonusly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonusly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.bonus.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bonus.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bonusly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bonus.ly\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/security/bonusly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employee Recognition
- Rewards
- Employee Engagement
- HR
- Company Culture
- Bonuses
---
