---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weave.works
  spf: false
hosts:
- cert_expires: Sep 23 06:12:56 2026 GMT
  host: www.weave.works
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weaveworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weaveworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Weaveworks
provider_slug: weaveworks
slug: weaveworks-domain-security
source_filename: weaveworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weave.works\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:12:56 2026 GMT\n  hsts: null\ndomains:\n- domain: weave.works\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weaveworks/refs/heads/main/security/weaveworks-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Developer Tools
- GitOps
- Kubernetes
- Container Networking
- Cloud Native
- Open Source
- DevOps
---
