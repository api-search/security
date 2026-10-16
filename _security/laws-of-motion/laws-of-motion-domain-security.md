---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lawsofmotion.com
  spf: true
hosts:
- cert_expires: Dec 27 17:36:32 2026 GMT
  host: lawsofmotion.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laws Of Motion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laws of Motion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laws of Motion
provider_slug: laws-of-motion
slug: laws-of-motion-domain-security
source_filename: laws-of-motion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawsofmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:36:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: lawsofmotion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laws-of-motion/refs/heads/main/security/laws-of-motion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- AI
- E-commerce
- Clothing
---
