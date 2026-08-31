---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.jobs
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.amazon.jobs
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiva Systems Amazon Robotics Since 2012 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiva Systems (Amazon Robotics since 2012), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kiva Systems (Amazon Robotics since 2012)
provider_slug: kiva-systems-amazon-robotics-since-2012
slug: kiva-systems-amazon-robotics-since-2012-domain-security
source_filename: kiva-systems-amazon-robotics-since-2012-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amazon.jobs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47474747\ndomains:\n- domain: amazon.jobs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiva-systems-amazon-robotics-since-2012/refs/heads/main/security/kiva-systems-amazon-robotics-since-2012-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Ai
- Robotics
- Warehouse Automation
- Fulfillment
- Logistics
- Acquisition
- Amazon
---
