---
description: ''
domains:
- caa:
  - 0 iodef "mailto:it-security@mirantis.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mirantis.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: k0rdent.io
  spf: false
hosts:
- cert_expires: Dec 29 06:37:17 2026 GMT
  host: www.mirantis.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 05:39:23 2026 GMT
  host: k0rdent.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 18:18:21 2026 GMT
  host: k0sproject.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Mirantis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirantis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mirantis
provider_slug: mirantis
slug: mirantis-domain-security
source_filename: mirantis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirantis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 06:37:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: k0rdent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:39:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: k0sproject.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:18:21 2026 GMT\n  hsts: false\ndomains:\n- domain: mirantis.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it-security@mirantis.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: k0rdent.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirantis/refs/heads/main/security/mirantis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kubernetes
- Containers
- Cloud
- DevOps
- OpenStack
---
