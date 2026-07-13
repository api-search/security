---
api_specs:
- filename: architectural-design-patterns-api.yaml
  format: yaml
  label: Architectural Design Patterns API
  slug: architectural-design-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/openapi/architectural-design-patterns-api.yaml
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
name: Architectural Design Patterns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Architectural Design Patterns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
slug: architectural-design-patterns-domain-security
source_filename: architectural-design-patterns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/security/architectural-design-patterns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
---
