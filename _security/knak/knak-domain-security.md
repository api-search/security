---
api_specs:
- filename: knak-enterprise-openapi-original.yml
  format: yaml
  label: Knak Enterprise API
  slug: enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-enterprise-openapi-original.yml
- filename: knak-send-openapi-original.yml
  format: yaml
  label: Knak Send Contacts API
  slug: send
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-send-openapi-original.yml
- filename: knak-scim-openapi-original.yml
  format: yaml
  label: Knak SCIM API
  slug: scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-scim-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knak.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knak.io
  spf: true
hosts:
- cert_expires: Sep 24 09:10:10 2026 GMT
  host: knak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 18:06:35 2026 GMT
  host: developer.knak.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: enterprise.knak.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knak, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knak
provider_slug: knak
slug: knak-domain-security
source_filename: knak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:10:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.knak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:06:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enterprise.knak.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: knak.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: knak.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\
  \n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/security/knak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Marketing
- Marketing Automation
- Landing Pages
- Content Creation
- Marketing Operations
- Campaign Management
- No-Code
- SCIM
- Webhooks
---
