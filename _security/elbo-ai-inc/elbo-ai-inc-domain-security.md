---
api_specs:
- filename: elbo-ai-inc-puppetry-openapi-original.json
  format: json
  label: Puppetry Developer API
  slug: puppetry-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elbo-ai-inc/refs/heads/main/openapi/elbo-ai-inc-puppetry-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: puppetry.com
  spf: true
hosts:
- cert_expires: Sep  9 10:21:47 2026 GMT
  host: puppetry.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:26:23 2026 GMT
  host: www.puppetry.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elbo Ai Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELBO AI, INC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ELBO AI, INC
provider_slug: elbo-ai-inc
slug: elbo-ai-inc-domain-security
source_filename: elbo-ai-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: puppetry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:21:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.puppetry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:26:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: puppetry.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elbo-ai-inc/refs/heads/main/security/elbo-ai-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Text to Speech
- Voice
- Generative AI
- Avatars
- Content Creation
- Developer API
- MCP
---
