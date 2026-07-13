---
api_specs:
- filename: affinity-v2-openapi.yml
  format: yaml
  label: Affinity API V2
  slug: affinity-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affinity.co
  spf: true
hosts:
- cert_expires: Aug 16 21:23:34 2026 GMT
  host: www.affinity.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 10:43:19 2026 GMT
  host: api-docs.affinity.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.affinity.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affinity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Affinity
provider_slug: affinity
slug: affinity-domain-security
source_filename: affinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affinity.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.affinity.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:43:19 2026 GMT\n  hsts: false\n- host: api.affinity.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: affinity.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/security/affinity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Relationship Intelligence
- Private Equity
- Venture Capital
- Contacts
- Organizations
- Opportunities
- Deal Management
---
