---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognizant.com
  spf: true
hosts:
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: www.cognizant.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognizant Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognizant Technology Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognizant Technology Solutions
provider_slug: cognizant-technology
slug: cognizant-technology-domain-security
source_filename: cognizant-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognizant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: cognizant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognizant-technology/refs/heads/main/security/cognizant-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Platform
- Consulting
- Digital Transformation
- IT Services
- Multi-Agent
- Neuro AI
- Fortune 500
---
