---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:GISIIPCertificatePlatformsAdmin@barclayscorp.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barclays.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: developer.barclays.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barclays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barclays, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barclays
provider_slug: barclays
slug: barclays-domain-security
source_filename: barclays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.barclays.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: barclays.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:GISIIPCertificatePlatformsAdmin@barclayscorp.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barclays/refs/heads/main/security/barclays-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
---
