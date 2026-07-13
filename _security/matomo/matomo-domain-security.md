---
api_specs:
- filename: matomo-openapi.yml
  format: yaml
  label: Matomo Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/openapi/matomo-openapi.yml
- filename: matomo-tracking-openapi.yml
  format: yaml
  label: Matomo Tracking API
  slug: tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/openapi/matomo-tracking-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: matomo.org
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: matomo.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: developer.matomo.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matomo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matomo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matomo
provider_slug: matomo
slug: matomo-domain-security
source_filename: matomo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matomo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.matomo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: matomo.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matomo/refs/heads/main/security/matomo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data Ownership
- Open Source
- Privacy
- Self-Hosted
- Web Analytics
---
