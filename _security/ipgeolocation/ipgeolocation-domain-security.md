---
api_specs:
- filename: ipgeolocation-ip-location-openapi.yml
  format: yaml
  label: IP Geolocation
  slug: ip-geolocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-location-openapi.yml
- filename: ipgeolocation-security-openapi.yml
  format: yaml
  label: IP Security
  slug: ip-security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-security-openapi.yml
- filename: ipgeolocation-asn-openapi.yml
  format: yaml
  label: ASN Lookup
  slug: asn-lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-asn-openapi.yml
- filename: ipgeolocation-abuse-openapi.yml
  format: yaml
  label: IP Abuse Contact
  slug: ip-abuse-contact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-abuse-openapi.yml
- filename: ipgeolocation-timezone-openapi.yml
  format: yaml
  label: Timezone
  slug: timezone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-timezone-openapi.yml
- filename: ipgeolocation-astronomy-openapi.yml
  format: yaml
  label: Astronomy
  slug: astronomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-astronomy-openapi.yml
- filename: ipgeolocation-user-agent-openapi.yml
  format: yaml
  label: User Agent
  slug: user-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-user-agent-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ipgeolocation.io
  spf: true
hosts:
- cert_expires: Aug 16 08:21:00 2026 GMT
  host: ipgeolocation.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 16 06:09:55 2026 GMT
  host: api.ipgeolocation.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipgeolocation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPGeolocation.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IPGeolocation.io
provider_slug: ipgeolocation
slug: ipgeolocation-domain-security
source_filename: ipgeolocation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipgeolocation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:21:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ipgeolocation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 16 06:09:55 2026 GMT\n  hsts: false\ndomains:\n- domain: ipgeolocation.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/security/ipgeolocation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
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
