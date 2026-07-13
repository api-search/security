---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uaeu.ac.ae
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: fcsc.gov.ae
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.uaeu.ac.ae
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 11:22:13 2026 GMT
  host: scholarworks.uaeu.ac.ae
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:27:00 2026 GMT
  host: opendata.fcsc.gov.ae
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United Arab Emirates University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Arab Emirates University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: United Arab Emirates University
provider_slug: united-arab-emirates-university
slug: united-arab-emirates-university-domain-security
source_filename: united-arab-emirates-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uaeu.ac.ae\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: scholarworks.uaeu.ac.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:22:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opendata.fcsc.gov.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:27:00 2026 GMT\n  hsts: null\ndomains:\n- domain: uaeu.ac.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fcsc.gov.ae\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-arab-emirates-university/refs/heads/main/security/united-arab-emirates-university-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Institutional Repository
- OAI-PMH
- CKAN
- United Arab Emirates
- Middle East
---
