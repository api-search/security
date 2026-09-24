---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huawei.com
  spf: true
hosts:
- cert_expires: Nov 27 08:01:06 2026 GMT
  host: solar.huawei.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Huawei Fusionsolar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huawei FusionSolar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Huawei FusionSolar
provider_slug: huawei-fusionsolar
slug: huawei-fusionsolar-domain-security
source_filename: huawei-fusionsolar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solar.huawei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 08:01:06 2026 GMT\n  hsts: false\ndomains:\n- domain: huawei.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huawei-fusionsolar/refs/heads/main/security/huawei-fusionsolar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Solar
- Energy
- IoT
- Inverters
---
