---
description: ''
domains:
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: icloud.com
  spf: true
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Jan  7 18:07:22 2027 GMT
  host: www.icloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 20:54:06 2027 GMT
  host: api.apple-cloudkit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple CloudKit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple CloudKit
provider_slug: cloudkit
slug: cloudkit-domain-security
source_filename: cloudkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 18:07:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apple-cloudkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 20:54:06 2027 GMT\n  hsts: null\ndomains:\n- domain: icloud.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/security/cloudkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apple
- Cloud Storage
- CloudKit
- Database
- iCloud
- Mobile
- Sync
- Web Services
---
