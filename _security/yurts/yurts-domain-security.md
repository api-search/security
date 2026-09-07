---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: legionintel.com
  spf: true
hosts:
- cert_expires: Nov 16 07:39:30 2026 GMT
  host: www.legionintel.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yurts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yurts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yurts
provider_slug: yurts
slug: yurts-domain-security
source_filename: yurts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.legionintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 07:39:30 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: legionintel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yurts/refs/heads/main/security/yurts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Agentic AI
- National Security
- Defense
- Generative AI
- Enterprise Search
- Retrieval Augmented Generation
- Edge AI
- Government
---
