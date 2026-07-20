---
api_specs:
- filename: docs
  format: yaml
  label: Craft.io Workspace API
  slug: craftio-workspace-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Portfolio API
  slug: craftio-portfolio-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Feedback Portal API
  slug: craftio-feedback-portal-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: craft.io
  spf: true
hosts:
- cert_expires: Sep 17 23:52:00 2026 GMT
  host: craft.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:54:20 2026 GMT
  host: help.craft.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:54:20 2026 GMT
  host: api.craft.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craft Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craft.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Craft.io
provider_slug: craft-io
slug: craft-io-domain-security
source_filename: craft-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:52:00 2026 GMT\n  hsts: false\n- host: help.craft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:54:20 2026 GMT\n  hsts: false\n- host: api.craft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:54:20 2026 GMT\n  hsts: null\ndomains:\n- domain: craft.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craft-io/refs/heads/main/security/craft-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product Management
- Roadmaps
- OKRs
- Backlog
- Feedback
- Portfolio
- Specifications
---
