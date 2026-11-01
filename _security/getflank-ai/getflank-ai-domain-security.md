---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getflank.ai
  spf: true
hosts:
- cert_expires: Nov 30 19:56:53 2026 GMT
  host: www.getflank.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getflank Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Flank
provider_slug: getflank-ai
slug: getflank-ai-domain-security
source_filename: getflank-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getflank.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 19:56:53 2026 GMT\n  hsts: null\ndomains:\n- domain: getflank.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getflank-ai/security/getflank-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
