---
api_specs:
- filename: farmlogs-openapi.yml
  format: yaml
  label: FarmLogs Fields
  slug: fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/openapi/farmlogs-openapi.yml
- filename: farmlogs-openapi.yml
  format: yaml
  label: FarmLogs Satellite Imagery / NDVI
  slug: satellite-imagery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/openapi/farmlogs-openapi.yml
- filename: farmlogs-openapi.yml
  format: yaml
  label: FarmLogs Weather & Rainfall
  slug: weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/openapi/farmlogs-openapi.yml
- filename: farmlogs-openapi.yml
  format: yaml
  label: FarmLogs Yield & Profitability
  slug: yield-and-profitability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/openapi/farmlogs-openapi.yml
- filename: farmlogs-openapi.yml
  format: yaml
  label: FarmLogs Activities & Scouting
  slug: activities-and-scouting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/openapi/farmlogs-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: farmlogs.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:systems@bushelpowered.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bushelpowered.com
  spf: true
hosts:
- cert_expires: Aug 22 20:11:39 2026 GMT
  host: www.farmlogs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 04:23:57 2026 GMT
  host: bushelpowered.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmlogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FarmLogs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FarmLogs
provider_slug: farmlogs
slug: farmlogs-domain-security
source_filename: farmlogs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farmlogs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:11:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bushelpowered.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmlogs.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bushelpowered.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:systems@bushelpowered.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/security/farmlogs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Farm Management
- Precision Agriculture
- Satellite Imagery
- Acquired
- Discontinued Brand
---
