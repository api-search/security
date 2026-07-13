---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bizzabo.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Aug 20 10:56:40 2026 GMT
  host: www.bizzabo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: bizzabo.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 10:56:40 2026 GMT
  host: api.bizzabo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bizzabo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizzabo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bizzabo
provider_slug: bizzabo
slug: bizzabo-domain-security
source_filename: bizzabo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bizzabo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:56:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bizzabo.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bizzabo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:56:40 2026 GMT\n  hsts: null\ndomains:\n- domain: bizzabo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizzabo/refs/heads/main/security/bizzabo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Management
- B2B Events
- Conference Management
- Ticketing
- Attendees
- Speakers
- Registration
- Analytics
- Event Technology
---
