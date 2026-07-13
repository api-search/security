---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:caa@airship.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: airship.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caa@airship.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanairship.com
  spf: true
hosts:
- cert_expires: Aug 28 16:02:11 2026 GMT
  host: www.airship.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:32:03 2026 GMT
  host: docs.airship.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 20:52:32 2026 GMT
  host: go.urbanairship.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airship, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Airship
provider_slug: airship
slug: airship-domain-security
source_filename: airship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:02:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.airship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:32:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: go.urbanairship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:52:32 2026 GMT\n  hsts: null\ndomains:\n- domain: airship.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:caa@airship.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: urbanairship.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caa@airship.com\"\
  \n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/security/airship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Notifications
- Push
- Email
- Mobile
- CDP
---
