---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xiaoe-tech.com
  spf: true
hosts:
- cert_expires: Jan 28 00:59:59 2027 GMT
  host: www.xiaoe-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 00:59:59 2027 GMT
  host: api-doc.xiaoe-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.xiaoe-tech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiaoe (小鹅通), probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xiaoe (小鹅通)
provider_slug: sem
slug: sem-domain-security
source_filename: sem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xiaoe-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 00:59:59 2027 GMT\n  hsts: false\n- host: api-doc.xiaoe-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 00:59:59 2027 GMT\n  hsts: false\n- host: api.xiaoe-tech.com\n  https: false\ndomains:\n- domain: xiaoe-tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sem/refs/heads/main/security/sem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- Private Domain
- Content Commerce
- Live Streaming
- Education
- E-Commerce
- Marketing
- WeChat
- China
---
