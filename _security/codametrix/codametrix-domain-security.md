---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codametrix.com
  spf: true
hosts:
- cert_expires: Sep 10 15:01:35 2026 GMT
  host: www.codametrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 05:22:09 2026 GMT
  host: status.codametrix.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codametrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodaMetrix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodaMetrix
provider_slug: codametrix
slug: codametrix-domain-security
source_filename: codametrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codametrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.codametrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:22:09 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: codametrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/security/codametrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- healthcare
- health-systems
- medical-coding
- autonomous-coding
- revenue-cycle-management
- clinical-documentation
- healthcare-ai
- machine-learning
- natural-language-processing
- ehr-integration
- status
---
