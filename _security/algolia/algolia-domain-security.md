---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: algolia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: algolia.io
  spf: true
hosts:
- cert_expires: Oct  7 04:14:17 2026 GMT
  host: www.algolia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: insights.algolia.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 04:14:17 2026 GMT
  host: analytics.algolia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Algolia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algolia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Algolia
provider_slug: algolia
slug: algolia-domain-security
source_filename: algolia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.algolia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:14:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: insights.algolia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: analytics.algolia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:14:17 2026 GMT\n  hsts: null\ndomains:\n- domain: algolia.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: algolia.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/security/algolia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Discovery
- Recommendations
- Personalization
- Analytics
- Ecommerce
---
