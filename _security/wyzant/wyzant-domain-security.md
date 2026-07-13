---
api_specs:
- filename: wyzant-openapi.yml
  format: yaml
  label: Wyzant Tutor Search API
  slug: wyzant-tutor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/openapi/wyzant-openapi.yml
- filename: wyzant-openapi.yml
  format: yaml
  label: Wyzant Tutor Data Feed
  slug: wyzant-tutor-data-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/openapi/wyzant-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wyzant.com
  spf: true
hosts:
- cert_expires: Aug 25 15:49:11 2026 GMT
  host: www.wyzant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:49:11 2026 GMT
  host: support.wyzant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:49:11 2026 GMT
  host: data.wyzant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wyzant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wyzant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Wyzant
provider_slug: wyzant
slug: wyzant-domain-security
source_filename: wyzant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wyzant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:49:11 2026 GMT\n  hsts: false\n- host: support.wyzant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:49:11 2026 GMT\n  hsts: false\n- host: data.wyzant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:49:11 2026 GMT\n  hsts: false\ndomains:\n- domain: wyzant.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/security/wyzant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Tutoring
- Education
- Marketplace
- Tutors
- EdTech
- Affiliate
- Partner API
- Data Feed
---
