---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: emergentcf.cloud
  spf: true
hosts:
- host: emergentcf.cloud
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emergentcf Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for //HERE, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: //HERE
provider_slug: emergentcf-cloud
slug: emergentcf-cloud-domain-security
source_filename: emergentcf-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emergentcf.cloud\n  https: false\ndomains:\n- domain: emergentcf.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/emergentcf-cloud/security/emergentcf-cloud-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Agents
- A2A
- Agentic Commerce
- x402
- Stablecoins
---
