---
api_specs:
- filename: revinate-porter-openapi.yml
  format: yaml
  label: Revinate Porter API
  slug: porter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-porter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: revinate.com
  spf: true
hosts:
- cert_expires: Oct 28 09:37:43 2026 GMT
  host: www.revinate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: porter.revinate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revinate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revinate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Revinate
provider_slug: revinate
slug: revinate-domain-security
source_filename: revinate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revinate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 09:37:43 2026 GMT\n  hsts: false\n- host: porter.revinate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: revinate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/security/revinate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Hotels
- Reviews
- Reputation Management
- Guest Data Platform
- CRM
- Sentiment Analysis
- Travel
- Marketing
- Customer Feedback
---
