---
api_specs:
- filename: aimodel-content-wp-routes-original.json
  format: json
  label: AI model Website (WordPress REST)
  slug: ai-model-jp-website-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimodel/refs/heads/main/openapi/aimodel-content-wp-routes-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ai-model.jp
  spf: true
hosts:
- cert_expires: Oct 28 14:59:59 2026 GMT
  host: www.ai-model.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aimodel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI model, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AI model
provider_slug: aimodel
slug: aimodel-domain-security
source_filename: aimodel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ai-model.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 14:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ai-model.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimodel/refs/heads/main/security/aimodel-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Generative AI
- Japan
- E-Commerce
- Fashion
- Apparel
- Advertising
- Marketing
- Content
- Digital Human
- Media
- WordPress
---
