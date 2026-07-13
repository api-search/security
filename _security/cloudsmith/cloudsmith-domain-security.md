---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudsmith API (v1)
  slug: v1
  spec_type: OpenAPI
  url: https://api.cloudsmith.io/?format=openapi
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudsmith.com
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudsmith.io
  spf: true
hosts:
- cert_expires: Sep 11 06:46:09 2026 GMT
  host: cloudsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 09:04:00 2026 GMT
  host: docs.cloudsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.cloudsmith.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudsmith, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudsmith
provider_slug: cloudsmith
slug: cloudsmith-domain-security
source_filename: cloudsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cloudsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cloudsmith.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cloudsmith.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cloudsmith.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"\
  amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsmith/refs/heads/main/security/cloudsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifact Management
- DevOps
- DevSecOps
- Distribution
- Package Management
- Registry
- Repository
- Software Supply Chain
- Universal
- Vulnerability Scanning
---
