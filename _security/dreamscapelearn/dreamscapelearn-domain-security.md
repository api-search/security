---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dreamscapelearn.com
  spf: true
hosts:
- cert_expires: Jan  8 15:57:21 2027 GMT
  host: www.dreamscapelearn.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dreamscapelearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dreamscapelearn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dreamscapelearn
provider_slug: dreamscapelearn
slug: dreamscapelearn-domain-security
source_filename: dreamscapelearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dreamscapelearn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 15:57:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: dreamscapelearn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dreamscapelearn/security/dreamscapelearn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- VirtualReality
- ImmersiveLearning
- K-12
- HigherEducation
- Company
---
