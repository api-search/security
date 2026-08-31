---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openbao.org
  spf: true
hosts:
- cert_expires: Oct 26 06:17:20 2026 GMT
  host: openbao.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openbao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenBao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenBao
provider_slug: openbao
slug: openbao-domain-security
source_filename: openbao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openbao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 06:17:20 2026 GMT\n  hsts: false\ndomains:\n- domain: openbao.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openbao/refs/heads/main/security/openbao-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Secrets Management
- Security
- Identity and Access Management
- Encryption
- Certificates
- PKI
- Key Management
- Open-Source
- Self-Hosted
- Linux Foundation
- DevOps
- Infrastructure
---
