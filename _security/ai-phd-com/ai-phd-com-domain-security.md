---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ai-phd.com
  spf: true
hosts:
- cert_expires: Jan  5 08:00:55 2027 GMT
  host: ai-phd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI PhD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI PhD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AI PhD
provider_slug: ai-phd-com
slug: ai-phd-com-domain-security
source_filename: ai-phd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-phd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:00:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ai-phd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ai-phd-com/security/ai-phd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Artificial Intelligence
- Courses
- Learning
- Platform
---
