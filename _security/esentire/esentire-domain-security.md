---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: esentire.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.esentire.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.esentire.com
  hsts: true
  hsts_header: 'strict-transport-security: max-age=31536000 ; includeSubDomains'
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_version: HTTP/2
  https: true
  note: 'The automated probe recorded hsts: null because the host root answers 403 with no HSTS header. The header IS present on routed responses — observed on a 401 from https://api.esentire.com/mcp/v1 on 2026-08-12. Corrected here from that direct observation.'
  tls_version: TLSv1.3
- host: trust.esentire.com
  hsts: unknown
  https: true
  note: UpGuard-hosted trust center (CNAME to UpGuard infrastructure), not eSentire-operated.
kind: domain-security
layout: security
method: probed
name: Esentire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSentire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: eSentire
provider_slug: esentire
slug: esentire-domain-security
source_filename: esentire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esentire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.esentire.com\n  https: true\n  http_version: HTTP/2\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_header: 'strict-transport-security: max-age=31536000 ; includeSubDomains'\n  note: >-\n    The automated probe recorded hsts: null because the host root answers 403 with\n    no HSTS header. The header IS present on routed responses — observed on a 401\n    from https://api.esentire.com/mcp/v1 on 2026-08-12. Corrected here from that\n    direct observation.\n- host: trust.esentire.com\n  https: true\n  hsts: unknown\n  note: UpGuard-hosted trust center (CNAME to UpGuard infrastructure), not eSentire-operated.\ndomains:\n\
  - domain: esentire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esentire/refs/heads/main/security/esentire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Incident Response
- Model Context Protocol
- Agents
- OAuth
- SaaS
---
