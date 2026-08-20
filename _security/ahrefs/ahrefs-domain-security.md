---
api_specs:
- filename: ahrefs-openapi-original.json
  format: json
  label: Ahrefs API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/openapi/_original/ahrefs-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ahrefs.com
  spf: true
hosts:
- cert_expires: Oct 20 05:44:45 2026 GMT
  host: ahrefs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 05:44:45 2026 GMT
  host: docs.ahrefs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 05:44:45 2026 GMT
  host: api.ahrefs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ahrefs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ahrefs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ahrefs
provider_slug: ahrefs
slug: ahrefs-domain-security
source_filename: ahrefs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ahrefs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:44:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ahrefs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:44:45 2026 GMT\n  hsts: false\n- host: api.ahrefs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:44:45 2026 GMT\n  hsts: null\ndomains:\n- domain: ahrefs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/security/ahrefs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SEO
- Marketing
- Search
- Analytics
- Backlinks
- Keywords
- Web Analytics
- Rank Tracking
- Site Audit
- Brand Monitoring
- Social-Media
---
