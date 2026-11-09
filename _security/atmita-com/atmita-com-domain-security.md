---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atmita.com
  spf: true
hosts:
- cert_expires: Jan  9 20:35:59 2027 GMT
  host: atmita.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atmita Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmita, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Atmita
provider_slug: atmita-com
slug: atmita-com-domain-security
source_filename: atmita-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atmita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 20:35:59 2027 GMT\n  hsts: false\ndomains:\n- domain: atmita.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/atmita-com/security/atmita-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Automation
- Productivity
- Software-as-a-Service
- Agents
---
