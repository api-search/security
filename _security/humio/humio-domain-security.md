---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:ops@humio.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humio.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.humio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: library.humio.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 21:33:23 2026 GMT
  host: cloud.humio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humio
provider_slug: humio
slug: humio-domain-security
source_filename: humio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: library.humio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: cloud.humio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 21:33:23 2026 GMT\n  hsts: null\ndomains:\n- domain: humio.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:ops@humio.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humio/refs/heads/main/security/humio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Big Data
- Log Management
- Observability
- Logging
- SIEM
- Monitoring
- Security
---
