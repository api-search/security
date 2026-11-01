---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memoryapi.org
  spf: false
hosts:
- cert_expires: Jan 19 19:09:32 2027 GMT
  host: memoryapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memoryapi Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memoryapi-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: memoryapi-org
provider_slug: memoryapi-org
slug: memoryapi-org-domain-security
source_filename: memoryapi-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memoryapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:09:32 2027 GMT\n  hsts: false\ndomains:\n- domain: memoryapi.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/memoryapi-org/security/memoryapi-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Agents
- Blockchain
- Finance
- Marketplace
---
