---
api_specs:
- filename: hackmd-openapi-original.json
  format: json
  label: HackMD API
  slug: hackmd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:support@hackmd.io"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hackmd.io
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: hackmd.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hackmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HackMD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HackMD
provider_slug: hackmd
slug: hackmd-domain-security
source_filename: hackmd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hackmd.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hackmd.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:support@hackmd.io\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/security/hackmd-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Markdown
- Collaboration
- Documentation
- Note Taking
- Knowledge Base
- Productivity
- Content
---
