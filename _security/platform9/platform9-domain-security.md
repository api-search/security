---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: platform9.com
  spf: true
hosts:
- cert_expires: Oct 14 15:23:51 2026 GMT
  host: platform9.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 20:24:02 2026 GMT
  host: docs.platform9.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Platform9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platform9, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Platform9
provider_slug: platform9
slug: platform9-domain-security
source_filename: platform9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:23:51 2026 GMT\n  hsts: false\n- host: docs.platform9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: platform9.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform9/refs/heads/main/security/platform9-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Private Cloud
- OpenStack
- Kubernetes
- Virtualization
- IaaS
- VMware Migration
- Cloud Management
---
