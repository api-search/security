---
api_specs:
- filename: ipgeolocation-asn-lookup-api-openapi.yml
  format: yaml
  label: IPGeolocation.io ASN Lookup API
  slug: ipgeolocation-asn-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-asn-lookup-api-openapi.yml
- filename: ipgeolocation-astronomy-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Astronomy API
  slug: ipgeolocation-astronomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-astronomy-api-openapi.yml
- filename: ipgeolocation-ip-abuse-contact-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Abuse Contact API
  slug: ipgeolocation-ip-abuse-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-ip-abuse-contact-api-openapi.yml
- filename: ipgeolocation-ip-geolocation-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Geolocation API
  slug: ipgeolocation-ip-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-ip-geolocation-api-openapi.yml
- filename: ipgeolocation-ip-security-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Security API
  slug: ipgeolocation-ip-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-ip-security-api-openapi.yml
- filename: ipgeolocation-timezone-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Timezone API
  slug: ipgeolocation-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-timezone-api-openapi.yml
- filename: ipgeolocation-user-agent-api-openapi.yml
  format: yaml
  label: IPGeolocation.io User Agent API
  slug: ipgeolocation-user-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipgeolocation/openapi/ipgeolocation-user-agent-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ipgeolocation.io
  spf: true
hosts:
- cert_expires: Dec 15 06:29:37 2026 GMT
  host: ipgeolocation.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 21:48:11 2026 GMT
  host: api.ipgeolocation.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: IPGeolocation.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPGeolocation.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IPGeolocation.io
provider_slug: ipgeolocation
slug: ipgeolocation-domain-security
source_filename: ipgeolocation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipgeolocation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 06:29:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ipgeolocation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 21:48:11 2026 GMT\n  hsts: false\ndomains:\n- domain: ipgeolocation.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ipgeolocation/security/ipgeolocation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IP Geolocation
- IP Intelligence
- IP Security
- ASN Lookup
- Abuse Contact
- Timezone
- Astronomy
- User Agent
- Threat Intelligence
- Public APIs
---
