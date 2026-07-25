---
api_specs:
- filename: guardian-content-api-openapi.yml
  format: yaml
  label: The Guardian Content API
  slug: guardian-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-content-api-openapi.yml
- filename: guardian-editions-api-openapi.yml
  format: yaml
  label: The Guardian Editions API
  slug: guardian-editions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-editions-api-openapi.yml
- filename: guardian-sections-api-openapi.yml
  format: yaml
  label: The Guardian Sections API
  slug: guardian-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-sections-api-openapi.yml
- filename: guardian-tags-api-openapi.yml
  format: yaml
  label: The Guardian Tags API
  slug: guardian-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theguardian.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guardianapis.com
  spf: true
hosts:
- cert_expires: Sep 21 19:33:19 2026 GMT
  host: open-platform.theguardian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: content.guardianapis.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Guardian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Guardian, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Guardian
provider_slug: guardian
slug: guardian-domain-security
source_filename: guardian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-platform.theguardian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:33:19 2026 GMT\n  hsts: false\n- host: content.guardianapis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: theguardian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: guardianapis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/security/guardian-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Media
- Content
- Articles
- Journalism
---
