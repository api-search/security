---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agno.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: phidata.com
  spf: true
hosts:
- cert_expires: Aug 16 10:45:54 2026 GMT
  host: agno.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 21:13:17 2026 GMT
  host: www.phidata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 00:34:33 2026 GMT
  host: docs.agno.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phidata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phidata / Agno, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phidata / Agno
provider_slug: phidata
slug: phidata-domain-security
source_filename: phidata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 10:45:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.phidata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.agno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:34:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: phidata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phidata/refs/heads/main/security/phidata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Agno
- Phidata
- Python
- Framework
- Runtime
- AgentOS
- Multi-Agent
- Memory
- Tools
- Open Source
---
