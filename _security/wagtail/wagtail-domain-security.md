---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wagtail.org
  spf: true
hosts:
- cert_expires: Aug 22 20:01:52 2026 GMT
  host: wagtail.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:03:26 2026 GMT
  host: docs.wagtail.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wagtail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wagtail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wagtail
provider_slug: wagtail
slug: wagtail-domain-security
source_filename: wagtail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wagtail.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.wagtail.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:03:26 2026 GMT\n  hsts: false\ndomains:\n- domain: wagtail.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagtail/refs/heads/main/security/wagtail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Django
- Python
- Headless CMS
- Open Source
- REST API
- Pages
- Images
- Documents
---
