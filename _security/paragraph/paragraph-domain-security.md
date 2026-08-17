---
api_specs:
- filename: paragraph-analytics-api-openapi.yml
  format: yaml
  label: Paragraph analytics API
  slug: paragraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-analytics-api-openapi.yml
- filename: paragraph-auth-api-openapi.yml
  format: yaml
  label: Paragraph auth API
  slug: paragraph-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-auth-api-openapi.yml
- filename: paragraph-coins-api-openapi.yml
  format: yaml
  label: Paragraph coins API
  slug: paragraph-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-coins-api-openapi.yml
- filename: paragraph-discover-api-openapi.yml
  format: yaml
  label: Paragraph discover API
  slug: paragraph-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-discover-api-openapi.yml
- filename: paragraph-emails-api-openapi.yml
  format: yaml
  label: Paragraph emails API
  slug: paragraph-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-emails-api-openapi.yml
- filename: paragraph-me-api-openapi.yml
  format: yaml
  label: Paragraph me API
  slug: paragraph-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-me-api-openapi.yml
- filename: paragraph-posts-api-openapi.yml
  format: yaml
  label: Paragraph posts API
  slug: paragraph-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-posts-api-openapi.yml
- filename: paragraph-publications-api-openapi.yml
  format: yaml
  label: Paragraph publications API
  slug: paragraph-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-publications-api-openapi.yml
- filename: paragraph-subscribers-api-openapi.yml
  format: yaml
  label: Paragraph subscribers API
  slug: paragraph-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-subscribers-api-openapi.yml
- filename: paragraph-users-api-openapi.yml
  format: yaml
  label: Paragraph users API
  slug: paragraph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-users-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: paragraph.com
  spf: true
hosts:
- cert_expires: Oct 24 16:57:02 2026 GMT
  host: paragraph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:13:31 2026 GMT
  host: docs.paragraph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 04:29:47 2026 GMT
  host: public.api.paragraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paragraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragraph, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paragraph
provider_slug: paragraph
slug: paragraph-domain-security
source_filename: paragraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paragraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 16:57:02 2026 GMT\n  hsts: false\n- host: docs.paragraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:13:31 2026 GMT\n  hsts: false\n- host: public.api.paragraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 04:29:47 2026 GMT\n  hsts: null\ndomains:\n- domain: paragraph.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/security/paragraph-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Publishing
- Newsletters
- Web3
- Content
- Blogging
- Creator Economy
- API
---
