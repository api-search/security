---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thomsonreuters.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: legal.thomsonreuters.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Westlaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westlaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Westlaw
provider_slug: westlaw
slug: westlaw-domain-security
source_filename: westlaw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legal.thomsonreuters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thomsonreuters.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westlaw/refs/heads/main/security/westlaw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LegalTech
- Research
- AI
- ThomsonReuters
- Westlaw
---
