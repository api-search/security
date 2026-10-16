---
api_specs:
- filename: cfengine-openapi-generated.yml
  format: yaml
  label: Cfengine API
  slug: cfengine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/_ae-authored/cfengine-openapi-generated.yml
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfengine.com
  spf: true
hosts:
- cert_expires: Dec 23 21:02:03 2026 GMT
  host: cfengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cfengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cfengine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cfengine
provider_slug: cfengine
slug: cfengine-domain-security
source_filename: cfengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cfengine.com\n  dnssec: true\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/security/cfengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automation
- Infrastructure
- Security
- Compliance
---
