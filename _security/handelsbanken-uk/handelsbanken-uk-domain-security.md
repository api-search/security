---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:sirt@handelsbanken.se"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: handelsbanken.co.uk
  spf: true
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:sirt@handelsbanken.se"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: handelsbanken.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.handelsbanken.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: developer.handelsbanken.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.handelsbanken.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Handelsbanken Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handelsbanken UK, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Handelsbanken UK
provider_slug: handelsbanken-uk
slug: handelsbanken-uk-domain-security
source_filename: handelsbanken-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.handelsbanken.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\n- host: developer.handelsbanken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.handelsbanken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: handelsbanken.co.uk\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:sirt@handelsbanken.se\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: handelsbanken.com\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:sirt@handelsbanken.se\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handelsbanken-uk/refs/heads/main/security/handelsbanken-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Open Banking
- Financial Services
- PSD2
- Berlin Group
- NextGenPSD2
- Payments
- Account Information
- United Kingdom
- Fintech
---
