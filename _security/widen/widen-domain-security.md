---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Acquia DAM API v2
  slug: acquia-dam-api-v2
  spec_type: OpenAPI
  url: https://widenv2.docs.apiary.io/
- filename: openapi.yaml
  format: yaml
  label: Acquia DAM API v1
  slug: acquia-dam-api-v1
  spec_type: OpenAPI
  url: https://widenv1.docs.apiary.io/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acquia.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: widencollective.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.acquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: docs.acquia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.widencollective.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Widen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Widen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Widen
provider_slug: widen
slug: widen-domain-security
source_filename: widen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acquia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acquia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.widencollective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: acquia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: widencollective.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/security/widen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Metadata
- Collections
- Workflows
- Acquia
---
