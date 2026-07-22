---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucloud.cn
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.ucloud.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: docs.ucloud.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.ucloud.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ucloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UCloud
provider_slug: ucloud
slug: ucloud-domain-security
source_filename: ucloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucloud.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: docs.ucloud.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.ucloud.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ucloud.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucloud/refs/heads/main/security/ucloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Cloud Computing
- IaaS
- GPU
- Kubernetes
- Object Storage
- CDN
- China
---
