---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autogenai.com
  spf: true
hosts:
- cert_expires: Dec 22 08:41:44 2026 GMT
  host: autogenai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autogenai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autogenai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autogenai
provider_slug: autogenai
slug: autogenai-domain-security
source_filename: autogenai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autogenai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:41:44 2026 GMT\n  hsts: false\ndomains:\n- domain: autogenai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autogenai/refs/heads/main/security/autogenai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- ProposalWriting
- Enterprise
- Government
- SaaS
---
