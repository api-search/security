---
api_specs:
- filename: seven-io-openapi-generated.yml
  format: yaml
  label: seven.io API
  slug: seven-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-io/refs/heads/main/openapi/_ae-authored/seven-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:webmaster@seven.io"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seven.io
  spf: true
hosts:
- cert_expires: Nov 18 19:36:44 2026 GMT
  host: www.seven.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seven Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for seven.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: seven.io
provider_slug: seven-io
slug: seven-io-domain-security
source_filename: seven-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seven.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 19:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: seven.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:webmaster@seven.io\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seven-io/refs/heads/main/security/seven-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SMS
- Voice
- Messaging
- CPaaS
- Germany
---
