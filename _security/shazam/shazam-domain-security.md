---
api_specs:
- filename: shazam-rest-api-openapi.yml
  format: yaml
  label: Shazam REST API (RapidAPI)
  slug: shazam-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/openapi/shazam-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shazam.com
  spf: true
- caa:
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Aug 27 00:00:00 2026 GMT
  host: www.shazam.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shazam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shazam, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shazam
provider_slug: shazam
slug: shazam-domain-security
source_filename: shazam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shazam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shazam.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/security/shazam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Audio Recognition
- Song Identification
- Charts
- Artists
- Tracks
- Fingerprinting
---
