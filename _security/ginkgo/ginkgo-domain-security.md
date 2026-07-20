---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ginkgobioworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ginkgobioworks.ai
  spf: true
hosts:
- cert_expires: Sep 22 13:57:49 2026 GMT
  host: www.ginkgobioworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ginkgobioworks.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Ginkgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ginkgo Bioworks, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ginkgo Bioworks
provider_slug: ginkgo
slug: ginkgo-domain-security
source_filename: ginkgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ginkgobioworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ginkgobioworks.ai\n  https: false\ndomains:\n- domain: ginkgobioworks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ginkgobioworks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ginkgo/refs/heads/main/security/ginkgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Synthetic Biology
- Biotechnology
- Artificial Intelligence
- Machine Learning
- Protein Models
- Bioinformatics
- Inference API
---
