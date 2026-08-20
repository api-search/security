---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teladochealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: visitnow.org
  spf: true
hosts:
- cert_expires: Sep 27 22:07:56 2026 GMT
  host: www.teladochealth.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 10:19:24 2026 GMT
  host: demo.visitnow.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teladoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teladoc, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Teladoc
provider_slug: teladoc
slug: teladoc-domain-security
source_filename: teladoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teladochealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:07:56 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: demo.visitnow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:19:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: teladochealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: visitnow.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teladoc/refs/heads/main/security/teladoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Tech
- Telehealth
- Telemedicine
- Virtual Care
- Healthcare
- Behavioral Health
- Webhook
---
