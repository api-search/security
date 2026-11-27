---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: redra.ai
  spf: false
hosts:
- cert_expires: Feb 20 23:51:39 2027 GMT
  host: redra.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Redra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Redra
provider_slug: redra-ai
slug: redra-ai-domain-security
source_filename: redra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:51:39 2027 GMT\n  hsts: false\ndomains:\n- domain: redra.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/redra-ai/security/redra-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Finance
- LegalTech
- Settlement
- Company
---
