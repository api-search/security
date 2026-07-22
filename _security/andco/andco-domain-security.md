---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useandco.com
  spf: true
hosts:
- cert_expires: Oct 11 08:01:46 2026 GMT
  host: www.useandco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Andco
provider_slug: andco
slug: andco-domain-security
source_filename: andco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useandco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 08:01:46 2026 GMT\n  hsts: false\ndomains:\n- domain: useandco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andco/refs/heads/main/security/andco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal Tech
- Personal Injury
- Legal
- AI Agents
- Document Automation
- Y Combinator
---
