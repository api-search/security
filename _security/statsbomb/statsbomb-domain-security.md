---
description: ''
domains:
- caa:
  - 0 iodef "mailto:infrastructure@hudl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hudl.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: statsbombservices.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.hudl.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: data.statsbombservices.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Statsbomb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StatsBomb (Hudl), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StatsBomb (Hudl)
provider_slug: statsbomb
slug: statsbomb-domain-security
source_filename: statsbomb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hudl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: data.statsbombservices.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hudl.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:infrastructure@hudl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: statsbombservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsbomb/refs/heads/main/security/statsbomb-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Football
- Soccer
- Analytics
- Event Data
- Tracking
- xG
- On-Ball Value
- Hudl
---
