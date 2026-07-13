---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@cognism.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cognism.com
  spf: true
hosts:
- cert_expires: Aug 31 13:57:40 2026 GMT
  host: www.cognism.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 15:59:00 2026 GMT
  host: api.cognism.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognism Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognism, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cognism
provider_slug: cognism
slug: cognism-domain-security
source_filename: cognism-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognism.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:57:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cognism.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:59:00 2026 GMT\n  hsts: null\ndomains:\n- domain: cognism.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@cognism.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/security/cognism-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- GDPR
- Intent Data
---
