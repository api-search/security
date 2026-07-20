---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 iodef "mailto:caa-admin@engflow.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: engflow.com
  spf: true
hosts:
- cert_expires: Sep 16 05:56:19 2026 GMT
  host: www.engflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 04:28:34 2026 GMT
  host: docs.engflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Engflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EngFlow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EngFlow
provider_slug: engflow
slug: engflow-domain-security
source_filename: engflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.engflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:56:19 2026 GMT\n  hsts: null\n- host: docs.engflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 04:28:34 2026 GMT\n  hsts: false\ndomains:\n- domain: engflow.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 iodef \"mailto:caa-admin@engflow.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engflow/refs/heads/main/security/engflow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Remote Execution
- Remote Caching
- Build Systems
- Bazel
- CI/CD
- Developer Tools
- gRPC
- Protocol Buffers
- DevOps
- Continuous Integration
---
