---
api_specs:
- filename: api.github.com.json
  format: json
  label: Source Control APIs
  slug: source-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Development Life Cycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Development Life Cycle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software Development Life Cycle
provider_slug: software-development-life-cycle
slug: software-development-life-cycle-domain-security
source_filename: software-development-life-cycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-development-life-cycle/refs/heads/main/security/software-development-life-cycle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development Process
- Project Management
- SDLC
- Software Engineering
- DevOps
- CI/CD
---
