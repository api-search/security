---
api_specs:
- filename: cloudsmithio-openapi-generated.yml
  format: yaml
  label: Cloudsmithio API
  slug: cloudsmithio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/openapi/_ae-authored/cloudsmithio-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudsmith.com
  spf: true
hosts:
- cert_expires: Nov 11 22:33:10 2026 GMT
  host: cloudsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudsmithio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudsmithio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudsmithio
provider_slug: cloudsmithio
slug: cloudsmithio-domain-security
source_filename: cloudsmithio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 22:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cloudsmith.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/security/cloudsmithio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifact Management
- Software Supply Chain
- Security
- DevOps
- Cloud
---
