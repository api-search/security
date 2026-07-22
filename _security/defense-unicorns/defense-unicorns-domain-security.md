---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: defenseunicorns.com
  spf: true
hosts:
- cert_expires: Oct 10 10:43:49 2026 GMT
  host: www.defenseunicorns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Unicorns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Unicorns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Defense Unicorns
provider_slug: defense-unicorns
slug: defense-unicorns-domain-security
source_filename: defense-unicorns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defenseunicorns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: defenseunicorns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-unicorns/refs/heads/main/security/defense-unicorns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- DevSecOps
- Kubernetes
- Defense
- Software Delivery
- Compliance
- Open Source
- Air Gap
---
