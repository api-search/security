---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getapril.com
  spf: true
hosts:
- cert_expires: Dec  8 07:00:09 2026 GMT
  host: www.getapril.com
  hsts: true
  hsts_max_age: 3571000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aprilgetaprilcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aprilgetaprilcom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aprilgetaprilcom
provider_slug: aprilgetaprilcom
slug: aprilgetaprilcom-domain-security
source_filename: aprilgetaprilcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getapril.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 07:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 3571000\ndomains:\n- domain: getapril.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aprilgetaprilcom/refs/heads/main/security/aprilgetaprilcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Tax
- API
- Embedded
---
