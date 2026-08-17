---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: base.ai
  spf: true
hosts:
- cert_expires: Sep 22 18:55:49 2026 GMT
  host: www.base.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Base Ai
provider_slug: base-ai
slug: base-ai-domain-security
source_filename: base-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.base.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: base.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nadditional_hosts_probed:\n- host: go.base.ai\n  https: true\n  note: application host (Vite SPA); edge returns the HTML shell under 200 for every path\n- host: status.base.ai\n  https: true\n  note: Atlassian Statuspage vendor host\n- host: support.base.ai\n  https: true\n  note: HubSpot-hosted help center\n- host: trust.base.ai\n  https: false\n  tls_error: unable to get local issuer certificate\n  note: >-\n    Resolves to an AWS ELB in us-east-2 and 301s from http, but the HTTPS handshake fails\n    certificate verification (incomplete or mismatched chain), so the host is unreachable to a\n    normal client. Probed\
  \ 2026-08-13.\nnotes: >-\n  base.ai publishes SPF and DMARC (p=quarantine) and serves HSTS with a one-year max-age, but has\n  no DNSSEC and no CAA records. A trust.base.ai hostname exists in DNS but does not present a\n  verifiable certificate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-ai/refs/heads/main/security/base-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Customer-Led Growth
- Customer Success
- Customer Marketing
- Advocacy
- RevOps
- SaaS
---
