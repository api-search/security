---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sware.com
  spf: true
hosts:
- cert_expires: Sep 29 07:43:14 2026 GMT
  host: www.sware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sware Fka Btr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sware (fka BTR), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sware (fka BTR)
provider_slug: sware-fka-btr
slug: sware-fka-btr-domain-security
source_filename: sware-fka-btr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sware-fka-btr/refs/heads/main/security/sware-fka-btr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Validation
- GxP
- Compliance
- Quality Assurance
- Regulatory
- Pharmaceutical
- Artificial Intelligence
---
