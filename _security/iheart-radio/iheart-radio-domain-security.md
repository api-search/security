---
api_specs:
- filename: openapi.yml
  format: yaml
  label: iHeartRadio Catalog API
  slug: iheartradio-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iheart-radio/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: iHeartRadio Live Stations API
  slug: iheartradio-live-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iheart-radio/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: iHeartRadio Podcasts API
  slug: iheartradio-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iheart-radio/refs/heads/main/openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iheart.com
  spf: true
hosts:
- cert_expires: Mar  6 18:30:15 2027 GMT
  host: www.iheart.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.iheart.com
  https: false
- cert_expires: Mar  6 18:30:15 2027 GMT
  host: api.iheart.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Iheart Radio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iHeartRadio, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iHeartRadio
provider_slug: iheart-radio
slug: iheart-radio-domain-security
source_filename: iheart-radio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iheart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 18:30:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.iheart.com\n  https: false\n- host: api.iheart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 18:30:15 2027 GMT\n  hsts: null\ndomains:\n- domain: iheart.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iheart-radio/refs/heads/main/security/iheart-radio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Radio
- Podcasts
- Music
- Streaming
- Audio
- Live Radio
- Digital Media
---
