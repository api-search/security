---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ironshard.ai
  spf: true
hosts:
- cert_expires: Jan 23 08:54:27 2027 GMT
  host: ironshard.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IronShard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IronShard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: IronShard
provider_slug: ironshard-ai
slug: ironshard-ai-domain-security
source_filename: ironshard-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ironshard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 08:54:27 2027 GMT\n  hsts: false\ndomains:\n- domain: ironshard.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ironshard-ai/security/ironshard-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Storage
- Artificial Intelligence
- Cloud
- S3
- MCP
---
