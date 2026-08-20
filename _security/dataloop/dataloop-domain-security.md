---
description: ''
domains:
- caa:
  - 0 iodef "mailto:devops@dataloop.ai"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dataloop.ai
  spf: true
hosts:
- cert_expires: Oct 15 13:59:44 2026 GMT
  host: dataloop.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 04:47:16 2026 GMT
  host: docs.dataloop.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 12:24:28 2026 GMT
  host: gate.dataloop.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dataloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataLoop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DataLoop
provider_slug: dataloop
slug: dataloop-domain-security
source_filename: dataloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:59:44 2026 GMT\n  hsts: null\n- host: docs.dataloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:47:16 2026 GMT\n  hsts: null\n- host: gate.dataloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 12:24:28 2026 GMT\n  hsts: null\ndomains:\n- domain: dataloop.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devops@dataloop.ai\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataloop/refs/heads/main/security/dataloop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Machine-Learning
- Data Management
- Data Annotation
- MLOps
- Computer-Vision
- Generative AI
- Data Labeling
- Pipelines
- Serverless
- Enterprise Software
- Company
---
