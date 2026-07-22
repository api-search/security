---
description: ''
domains:
- caa:
  - 0 iodef "mailto:devops@ceres.ai"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ceres.ai
  spf: true
hosts:
- cert_expires: Oct  8 03:35:23 2026 GMT
  host: ceres.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceresai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CeresAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CeresAI
provider_slug: ceresai
slug: ceresai-domain-security
source_filename: ceresai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceres.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:35:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ceres.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devops@ceres.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceresai/refs/heads/main/security/ceresai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Geospatial
- Remote Sensing
- Satellite Imagery
- Machine Learning
- Crop Health
- Agricultural Intelligence
- Insurance
---
