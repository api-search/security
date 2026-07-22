---
api_specs:
- filename: root-fka-slimai-openapi-original.json
  format: json
  label: Root.io API
  slug: rootio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root-fka-slimai/refs/heads/main/openapi/root-fka-slimai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: root.io
  spf: true
hosts:
- cert_expires: Oct  9 16:30:10 2026 GMT
  host: www.root.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:59:05 2026 GMT
  host: api.root.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Root Fka Slimai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Root (fka Slim.ai), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Root (fka Slim.ai)
provider_slug: root-fka-slimai
slug: root-fka-slimai-domain-security
source_filename: root-fka-slimai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.root.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:30:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.root.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:59:05 2026 GMT\n  hsts: null\ndomains:\n- domain: root.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root-fka-slimai/refs/heads/main/security/root-fka-slimai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Vulnerability Management
- Container Security
- DevSecOps
- Software Supply Chain
- CVE
- SBOM
- Open Source
- Patching
---
