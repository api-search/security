---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:ca.administrator@philips.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: philips.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hsdp.io
  spf: true
hosts:
- cert_expires: Aug 31 18:33:14 2026 GMT
  host: www.philips.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.hsdp.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Philips Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Philips, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Philips
provider_slug: philips
slug: philips-domain-security
source_filename: philips-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.philips.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 18:33:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hsdp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: philips.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:ca.administrator@philips.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hsdp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philips/refs/heads/main/security/philips-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Devices
- Connected Care
- Patient Monitoring
- HealthSuite
- HSDP
- Imaging
- IoT
- Cloud Platform
---
