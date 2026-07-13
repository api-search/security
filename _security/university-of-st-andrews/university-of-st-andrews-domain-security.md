---
api_specs:
- filename: university-of-st-andrews-status.yaml
  format: yaml
  label: Service Status API
  slug: status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-st-andrews/refs/heads/main/openapi/university-of-st-andrews-status.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: st-andrews.ac.uk
  spf: true
hosts:
- cert_expires: Aug 19 23:16:20 2026 GMT
  host: www.st-andrews.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 16:18:02 2026 GMT
  host: status.st-andrews.ac.uk
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:28:29 2026 GMT
  host: research-portal.st-andrews.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of St Andrews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of St Andrews, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of St Andrews
provider_slug: university-of-st-andrews
slug: university-of-st-andrews-domain-security
source_filename: university-of-st-andrews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.st-andrews.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.st-andrews.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: research-portal.st-andrews.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:28:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: st-andrews.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-st-andrews/refs/heads/main/security/university-of-st-andrews-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- OAI-PMH
- Scotland
- United Kingdom
---
