---
api_specs:
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Country Web Service
  slug: geoip-country
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP City Plus Web Service
  slug: geoip-city
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Insights Web Service
  slug: geoip-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Score
  slug: minfraud-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Insights
  slug: minfraud-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Factors
  slug: minfraud-factors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maxmind.com
  spf: true
hosts:
- cert_expires: Oct  1 11:00:03 2026 GMT
  host: www.maxmind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:57:42 2026 GMT
  host: dev.maxmind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 22:15:15 2026 GMT
  host: geoip.maxmind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maxmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaxMind, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MaxMind
provider_slug: maxmind
slug: maxmind-domain-security
source_filename: maxmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maxmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.maxmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:57:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: geoip.maxmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maxmind.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/security/maxmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IP Intelligence
- Geolocation
- Fraud Prevention
- Risk Scoring
- VPN Detection
- Proxy Detection
- ISP Data
- GeoIP
---
