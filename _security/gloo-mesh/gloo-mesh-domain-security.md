---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solo.io
  spf: true
hosts:
- cert_expires: Aug 16 06:19:48 2026 GMT
  host: www.solo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:29:55 2026 GMT
  host: docs.solo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gloo Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gloo Mesh, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gloo Mesh
provider_slug: gloo-mesh
slug: gloo-mesh-domain-security
source_filename: gloo-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:19:48 2026 GMT\n  hsts: false\n- host: docs.solo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:29:55 2026 GMT\n  hsts: false\ndomains:\n- domain: solo.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo-mesh/refs/heads/main/security/gloo-mesh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Istio
- Kubernetes
- Multi-Cluster
- Open Source
- Service Mesh
---
