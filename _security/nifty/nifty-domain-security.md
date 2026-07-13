---
api_specs:
- filename: source.yaml
  format: yaml
  label: Nifty Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://developers.niftypm.com/source.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: niftypm.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: niftypm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 03:43:08 2026 GMT
  host: developers.niftypm.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: openapi.niftypm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nifty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nifty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nifty
provider_slug: nifty
slug: nifty-domain-security
source_filename: nifty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: niftypm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\n- host: developers.niftypm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:43:08 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: openapi.niftypm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: niftypm.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nifty/refs/heads/main/security/nifty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Roadmaps
- Team Workspace
---
