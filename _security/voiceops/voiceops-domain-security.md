---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: voiceops.com
  spf: true
hosts:
- cert_expires: Oct 14 16:53:26 2026 GMT
  host: www.voiceops.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: mcp.voiceops.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- csp: true
  host: app.voiceops.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  source: manual probe (not an apis.yml baseURL host)
  x_frame_options: SAMEORIGIN
- host: api.voiceops.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  source: manual probe (not an apis.yml baseURL host)
  x_frame_options: DENY
kind: domain-security
layout: security
method: probed
name: Voiceops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VoiceOps, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VoiceOps
provider_slug: voiceops
slug: voiceops-domain-security
source_filename: voiceops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voiceops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:53:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.voiceops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\n- host: app.voiceops.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  csp: true\n  x_frame_options: SAMEORIGIN\n  source: manual probe (not an apis.yml baseURL host)\n- host: api.voiceops.com\n  https: true\n  hsts: true\n  hsts_max_age: 15768000\n  x_frame_options: DENY\n  source: manual probe (not an apis.yml baseURL host)\ncertificate:\n  issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M01\n  subject: CN=projectfrontline.net\n  not_before: Jul 12 00:00:00 2026 GMT\n  not_after: Jan 25 23:59:59 2027 GMT\n  subject_alt_names:\n  - projectfrontline.net\n  - '*.projectfrontline.net'\n\
  \  - app.voiceops.com\n  - '*.app.voiceops.com'\n  - api.voiceops.com\n  - mcp.voiceops.com\n  note: >-\n    One certificate fronts the application, API and MCP hosts. This is the\n    ownership evidence used throughout this profile.\nfindings:\n- >-\n  mcp.voiceops.com — the company's only public programmatic surface — returns no\n  Strict-Transport-Security header, while the marketing site, application and\n  API host all do.\n- No CAA records and no DNSSEC on voiceops.com.\n- DMARC policy is p=quarantine rather than p=reject.\ndomains:\n- domain: voiceops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceops/refs/heads/main/security/voiceops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Conversation Intelligence
- Call Centers
- Sales Coaching
- Customer Experience
- Artificial Intelligence
- Speech Analytics
- Model Context Protocol
- Agents
---
