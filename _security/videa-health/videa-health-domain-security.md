---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  - 0 iodef "mailto:devops@videa.ai"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: videa.ai
  spf: true
hosts:
- cert_expires: Aug 16 18:22:49 2026 GMT
  host: www.videa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Videa Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideaHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VideaHealth
provider_slug: videa-health
slug: videa-health-domain-security
source_filename: videa-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.videa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: videa.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:devops@videa.ai\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videa-health/refs/heads/main/security/videa-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dental
- Healthcare
- Artificial Intelligence
- Medical Imaging
- Radiograph Analysis
- Diagnostics
- Computer Vision
- FDA Cleared
- Gated API
---
