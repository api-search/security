---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vian.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vianai.site
  spf: false
hosts:
- cert_expires: Sep 10 05:02:05 2026 GMT
  host: www.vian.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:45:49 2026 GMT
  host: docs.vian.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: webservices.company.vianai.site
  https: false
kind: domain-security
layout: security
method: probed
name: Vianai Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vianai Systems, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vianai Systems
provider_slug: vianai-systems
slug: vianai-systems-domain-security
source_filename: vianai-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vian.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vian.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:45:49 2026 GMT\n  hsts: false\n- host: webservices.company.vianai.site\n  https: false\ndomains:\n- domain: vian.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vianai.site\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vianai-systems/refs/heads/main/security/vianai-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- MLOps
- Model Monitoring
- Analytics
- Generative AI
- Observability
- Conversational Analytics
---
