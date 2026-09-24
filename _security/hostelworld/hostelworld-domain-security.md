---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "certainly.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hostelworld.com
  spf: true
hosts:
- cert_expires: Dec 19 13:46:01 2026 GMT
  host: hostelworld.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hostelworld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostelworld, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hostelworld
provider_slug: hostelworld
slug: hostelworld-domain-security
source_filename: hostelworld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostelworld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 13:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hostelworld.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostelworld/refs/heads/main/security/hostelworld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Accommodation
- Booking
- Hospitality
---
