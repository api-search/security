---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mimikflow.com
  spf: true
hosts:
- cert_expires: Feb  2 12:13:16 2027 GMT
  host: mimikflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MimikFlow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MimikFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MimikFlow
provider_slug: mimikflow-com
slug: mimikflow-com-domain-security
source_filename: mimikflow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mimikflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 12:13:16 2027 GMT\n  hsts: false\ndomains:\n- domain: mimikflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mimikflow-com/security/mimikflow-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Sales
- Lead Generation
- Automation
- B2B
---
