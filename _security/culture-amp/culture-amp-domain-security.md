---
api_specs:
- filename: spec
  format: yaml
  label: Culture Amp Public API
  slug: culture-amp-public-api
  spec_type: OpenAPI
  url: https://api.cultureamp.com/spec
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@cultureamp.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cultureamp.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:security@cultureamp.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cultureamp.net
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.cultureamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.cultureamp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: sandbox.public-api.development.cultureamp.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Culture Amp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Culture Amp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Culture Amp
provider_slug: culture-amp
slug: culture-amp-domain-security
source_filename: culture-amp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cultureamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cultureamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.public-api.development.cultureamp.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cultureamp.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@cultureamp.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cultureamp.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:security@cultureamp.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/security/culture-amp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Human Resources
---
