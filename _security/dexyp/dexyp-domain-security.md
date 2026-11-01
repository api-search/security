---
description: ''
domains:
- caa:
  - 255 issue "digicert.com"
  - 255 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 254 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thryv.com
  spf: true
hosts:
- cert_expires: Nov 28 18:02:48 2026 GMT
  host: www.thryv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dexyp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexyp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dexyp
provider_slug: dexyp
slug: dexyp-domain-security
source_filename: dexyp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thryv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 18:02:48 2026 GMT\n  hsts: null\ndomains:\n- domain: thryv.com\n  dnssec: false\n  caa:\n  - 255 issue \"digicert.com\"\n  - 255 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 254 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dexyp/security/dexyp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Software
- Software-as-a-Service
- CRM
- Marketing Automation
- Workflow Optimization
---
