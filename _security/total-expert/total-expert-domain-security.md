---
api_specs:
- filename: total-expert-openapi.yml
  format: yaml
  label: Total Expert Public API
  slug: total-expert-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: totalexpert.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: totalexpert.net
  spf: true
hosts:
- cert_expires: Sep  1 22:09:48 2026 GMT
  host: totalexpert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: public.totalexpert.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: public.vt.totalexpert.net
  https: false
kind: domain-security
layout: security
method: probed
name: Total Expert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Total Expert, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Total Expert
provider_slug: total-expert
slug: total-expert-domain-security
source_filename: total-expert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: totalexpert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:09:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.totalexpert.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: public.vt.totalexpert.net\n  https: false\ndomains:\n- domain: totalexpert.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: totalexpert.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/security/total-expert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- CRM
- Marketing Automation
- Mortgage
- Banking
- Lending
- Customer Engagement
---
