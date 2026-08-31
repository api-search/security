---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:domains@free-now.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: free-now.com
  spf: true
hosts:
- cert_expires: Oct  8 21:08:18 2026 GMT
  host: www.free-now.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:49:02 2026 GMT
  host: developer.free-now.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.free-now.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Free Now Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FREE NOW, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FREE NOW
provider_slug: free-now
slug: free-now-domain-security
source_filename: free-now-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.free-now.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:08:18 2026 GMT\n  hsts: null\n- host: developer.free-now.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.free-now.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: free-now.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:domains@free-now.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-now/refs/heads/main/security/free-now-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobility
- Ride Hailing
- Transportation
- Taxi
- Mobility as a Service
- Travel
- Business
- Company
---
