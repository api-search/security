---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: celeryq.dev
  spf: true
hosts:
- cert_expires: Oct  3 06:44:00 2026 GMT
  host: docs.celeryq.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Celery
provider_slug: celery
slug: celery-domain-security
source_filename: celery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.celeryq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:44:00 2026 GMT\n  hsts: false\ndomains:\n- domain: celeryq.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celery/refs/heads/main/security/celery-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Asynchronous
- Distributed Systems
- Message Queue
- Open Source
- Python
- Task Queue
---
