---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vecnarobotics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: site.com
  spf: true
hosts:
- cert_expires: Oct 12 05:56:45 2026 GMT
  host: www.vecnarobotics.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:39:33 2026 GMT
  host: vecnarobotics.my.site.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vecna Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vecna Robotics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vecna Robotics
provider_slug: vecna-robotics
slug: vecna-robotics-domain-security
source_filename: vecna-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vecnarobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:56:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: vecnarobotics.my.site.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vecnarobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: site.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vecna-robotics/refs/heads/main/security/vecna-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Warehouse Automation
- Autonomous Mobile Robots
- Material Handling
- Logistics
- Supply Chain
- Manufacturing
- Industrial Automation
- Robotics as a Service
---
