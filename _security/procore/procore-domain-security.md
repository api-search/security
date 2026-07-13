---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security+domains@procore.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: procore.com
  spf: true
hosts:
- cert_expires: Sep 16 04:10:31 2026 GMT
  host: www.procore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 06:24:56 2026 GMT
  host: api.procore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Procore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procore, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Procore
provider_slug: procore
slug: procore-domain-security
source_filename: procore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.procore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:10:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.procore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:24:56 2026 GMT\n  hsts: null\ndomains:\n- domain: procore.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security+domains@procore.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procore/refs/heads/main/security/procore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Project Management
- Construction Management
- Field Productivity
- Financial Management
---
