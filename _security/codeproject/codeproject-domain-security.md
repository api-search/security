---
api_specs:
- filename: codeproject-rest-api-openapi.yml
  format: yaml
  label: CodeProject REST API
  slug: codeproject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-rest-api-openapi.yml
- filename: codeproject-ai-server-openapi.yml
  format: yaml
  label: CodeProject.AI Server API
  slug: codeproject-ai-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-ai-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codeproject.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: codeproject.ai
  spf: false
hosts:
- cert_expires: Oct 21 18:22:05 2026 GMT
  host: www.codeproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: codeproject.ai
  https: false
- host: api.codeproject.com
  https: false
kind: domain-security
layout: security
method: probed
name: Codeproject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeProject, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CodeProject
provider_slug: codeproject
slug: codeproject-domain-security
source_filename: codeproject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codeproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:22:05 2026 GMT\n  hsts: false\n- host: codeproject.ai\n  https: false\n- host: api.codeproject.com\n  https: false\ndomains:\n- domain: codeproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: codeproject.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/security/codeproject-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Articles
- Community
- Computer Vision
- Developer Community
- Face Recognition
- Forum
- Knowledge Base
- License Plate Recognition
- Object Detection
- Q&A
- Software Development
- Tutorials
---
