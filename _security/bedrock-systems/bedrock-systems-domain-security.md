---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bedrocksystems.com
  spf: true
hosts:
- cert_expires: Nov  4 05:13:00 2026 GMT
  host: www.bedrocksystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bedrock Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bedrock Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bedrock Systems
provider_slug: bedrock-systems
slug: bedrock-systems-domain-security
source_filename: bedrock-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bedrocksystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:13:00 2026 GMT\n  hsts: false\ndomains:\n- domain: bedrocksystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bedrock-systems/refs/heads/main/security/bedrock-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Hypervisor
- Virtualization
- Formal Verification
- Microhypervisor
- Open Source
---
