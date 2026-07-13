---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chainguard.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: enforce.dev
  spf: false
hosts:
- cert_expires: Sep 22 08:43:06 2026 GMT
  host: www.chainguard.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:11:16 2026 GMT
  host: edu.chainguard.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 18:39:08 2026 GMT
  host: console-api.enforce.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chainguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chainguard, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chainguard
provider_slug: chainguard
slug: chainguard-domain-security
source_filename: chainguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chainguard.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: edu.chainguard.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:11:16 2026 GMT\n  hsts: false\n- host: console-api.enforce.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:39:08 2026 GMT\n  hsts: null\ndomains:\n- domain: chainguard.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: enforce.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainguard/refs/heads/main/security/chainguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Native
- Container Images
- Containers
- DevSecOps
- Kubernetes
- Registry
- Security
- Software Supply Chain
- Vulnerability Management
---
