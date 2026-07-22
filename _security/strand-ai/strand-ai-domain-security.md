---
api_specs:
- filename: strand-ai-openapi-original.json
  format: json
  label: Strand Platform API
  slug: strand-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/openapi/strand-ai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: strandai.com
  spf: true
hosts:
- cert_expires: Oct  6 13:31:01 2026 GMT
  host: app.strandai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strand Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strand AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Strand AI
provider_slug: strand-ai
slug: strand-ai-domain-security
source_filename: strand-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.strandai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:31:01 2026 GMT\n  hsts: false\ndomains:\n- domain: strandai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strand-ai/refs/heads/main/security/strand-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Life Sciences
- Spatial Biology
- Bioinformatics
- Drug Discovery
- Foundation Models
- Digital Pathology
- Healthcare
---
