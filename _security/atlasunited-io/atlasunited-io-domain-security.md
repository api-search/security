---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@atlasunited.io"
  - 0 issue "hostinger.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atlasunited.io
  spf: true
hosts:
- cert_expires: Dec  3 07:08:49 2026 GMT
  host: atlasunited.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlas United Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas United, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atlas United
provider_slug: atlasunited-io
slug: atlasunited-io-domain-security
source_filename: atlasunited-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atlasunited.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 07:08:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atlasunited.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@atlasunited.io\"\n  - 0 issue \"hostinger.com\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/atlasunited-io/security/atlasunited-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Forecast
- Storm
- Geolocation
---
