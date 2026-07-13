---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yandex.com
  spf: true
hosts:
- cert_expires: Dec 29 20:59:59 2026 GMT
  host: yandex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yandex Weather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yandex.Weather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yandex.Weather
provider_slug: yandex-weather
slug: yandex-weather-domain-security
source_filename: yandex-weather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yandex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 20:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yandex.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yandex-weather/refs/heads/main/security/yandex-weather-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Public APIs
---
